# For Google workspace OAuth2 authentication

After 2022-10-04, Google workspace users connot use OAuth2 out-of-band
flow anymore. For mbsync and msmtp commands, you must use loopback IP flow
instead.
You can use `google-oauth2-loopback-ip.py` to get the refresh token,
and `google-oauth2-refresh-access_token.py` to get the access tokens
with the access token.

Please read [How to use Google Workspace OAuth2 with mbsync (from isync) and msmtp on NetBSD](https://blog.onodera.asia/2022/09/how-to-use-google-workspace-oauth2-with.html).

## Requirements
You can install required Python packages with [pkgsrc](https://www.pkgsrc.org/):

```
# cd /usr/pkgsrc/www/py-google-api-python-client
# make install
# cd /usr/pkgsrc/security/py-google-auth-oauthlib
# make install
```

## License
[Apache License Version 2.0](https://github.com/ryoon/google-oauth2-loopback-ip/blob/master/LICENSE)
