# Authentication
Everything you need to know about authenticating with the API.

## Headers
All requests require the following headers:
| Key             | Value                                                                                                                                             |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| User-Agent      | Mozilla/5.0 (Linux; U; Android 9; samsung SM-G950U; SmartHub Unknown; WIFI) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1 |
| requestsource   | SMARTHUB_ANDROID                                                                                                                                  |
| auth_source     | CIS                                                                                                                                               |
| accept-encoding | gzip                                                                                                                                              |

## Basic Authentication
All requests require the basic authentication header.

This header is a base64 encoded string of the following format:
```
email:password
```

Example:
| Key             | Value                                                           |
| --------------- | --------------------------------------------------------------  |
| authorization   | Basic: ZXhhbXBsZUBlbWFpbC5jb206UEFTU1dPUkRfSU5fUExBSU5fVEVYVA== |