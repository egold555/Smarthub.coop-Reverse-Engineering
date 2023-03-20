# Smarthub.coop Reverse Engineering
This is a collection of notes and information about the smarthub.coop JSON API.

------
## A Message to [NISC](https://www.nisc.coop/)

>In the U.S., Section 103(f) of the Digital Millennium Copyright Act (DMCA) [(17 USC § 1201 (f) - Reverse Engineering)](https://www.law.cornell.edu/uscode/text/17/1201) specifically states that it is legal to reverse engineer and circumvent the protection to achieve interoperability between computer programs (such as information transfer between applications). Interoperability is defined in paragraph 4 of Section 103(f).
>
>It is also often lawful to reverse-engineer an artifact or process as long as it is obtained legitimately. If the software is patented, it doesn't necessarily need to be reverse-engineered, as patents require a public disclosure of invention. It should be mentioned that, just because a piece of software is patented, that does not mean the entire thing is patented; there may be parts that remain undisclosed.

NISC, as coders we want to be able to use the smart meter data in other applications, like [Home Assistant](https://www.home-assistant.io/). You don't currently offer an official public API, so I have spent some time reverse engineering the [Android Companion App](https://play.google.com/store/apps/details?id=coop.nisc.android.smarthub&hl=en_US)'s API.

TL;DR, __please don't sue me, any contributors, or DMCA this repo__. If you wish for me to take it down, __please email me or leave a issue on this repo stating that you would like it to be removed, and I will happily do so__.

With all that out of the way, on to the documentation!

## Table of Contents
**WIP: Please see [requests/](/requests/) folder for now**
- [Authorization & Header Information](./requests/00-authorization-and-headers.md) 
- [Login Request](./requests/01-login.md)
- Company Information
  - todo
- Customer Information
  - todo
- Misc
  - todo


## How I reverse engineered the API
### Download the Android App
Download the [APK from the Play Store](), and extract it using [APK Extractor](https://play.google.com/store/apps/details?id=com.ext.ui&hl=en_US). Or use Google to download the apk from another website that I can't specify.

### Patch the App
The app uses [OkHttp](https://square.github.io/okhttp/) to make HTTP requests, and Android 10 and newer won't allow for MITM attacks using self signed certificates. So we need to patch the app to allow for this.

I used [APK-MITM](https://github.com/shroudedcode/apk-mitm) to automate the patching process. You could also use [APK TOOL](https://ibotpeaches.github.io/Apktool/) to manually patch the app.

### Capture the traffic
Then, I used [PCAPdroid](https://github.com/emanuele-f/PCAPdroid) to capture the HTTPS traffic from the app. Make sure you enable the HTTPS certificate in the app settings.

### Analyze & view the traffic
Then once I have interacted with the app, I can view the traffic in [Wireshark](https://www.wireshark.org/).

To descript the https traffic in wireshark, you need to import the `sslkeylogfile.txt` file into wireshark. PCapdroid will automatically generate this file for you when you export the pcap file.

I also used [pcapandroid.lua](https://github.com/emanuele-f/PCAPdroid/blob/master/tools/pcapdroid.lua) addon for wireshark to show what app the traffic is from.


### Testing the API
I used [Postman](https://www.postman.com/) to test the endpoints from wireshark.