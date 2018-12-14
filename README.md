# Botkit Middleware to populate Facebook Messenger user info to a Botkit message
## Installation
Add github repo url to package.json

Example:
```js

var fbuser = require('botkit-middleware-fbuser')({
    accessToken:'<fb_access_token>',
    fields: ['first_name', 'last_name', 'locale', 'profile_pic','timezone','gender','is_payment_enabled'],
    logLevel:'error',
    storage: '<Botkit storage object>'
});


controller.middleware.receive.use(fbuser.receive)
```
A message object will have an additional field `user_profile` with the fields requested to Facebook API.

##Author

**Nathan Zylbersztejn**

Github: [@znat](https://github.com/snat)

### Support:

If you want the good work to continue please support us on

* [PAYPAL](https://www.paypal.me/ishandutta2007)
* [BITCOIN ADDRESS: 3LZazKXG18Hxa3LLNAeKYZNtLzCxpv1LyD](https://www.coinbase.com/join/5a8e4a045b02c403bc3a9c0c)
