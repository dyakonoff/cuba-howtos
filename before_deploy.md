# What should you do before deploying a CUBA application to Live

## Secure your REST services

By default all CUBA applications have [Generic REST endpoints](http://files.cuba-platform.com/swagger/) enabled.
However, default OAuth2 [client.id and client.secret](https://doc.cuba-platform.com/manual-6.8/rest_api_v2_ex_get_token.html) come from CUBA.platform jar. Although it's quite convenient in development time having that parameters the same for all your CUBA applications. I'd highly recommend to set at least your cuba.rest.client.secret in your web-app.properties to some long and brute-force-proof password before deploying your application to Live.
