# drupal-backbone
This is a collection of useful Backbone.js code for writing [RESTful](https://github.com/RESTful-Drupal/restful) Drupal web apps. Several components are included, and you may include only those you require.

## Prerequisites

* Drupal 7: https://www.drupal.org
* RESTful module v2.x: https://github.com/RESTful-Drupal/restful
* Backbone JS: http://backbonejs.org

Additionally, the code is intended for use with [Browserify](http://browserify.org), but this isn't mandatory.

## Included and planned components

### Utilities

###### Base64
Used by the `DrupalUser` model to generate basic auth tokens.

```js
var Base64 = require("./drupal-utils").Base64;
var encoded = Base64.encode(someString);
```

### User

###### DrupalUser and DrupalUsers
A Drupal user model and collection.

```js
var drupalUser = require('app/drupal-backbone/drupal-user').UserModel;
var drupalUsers = require('app/drupal-backbone/drupal-user').UsersCollection;
```

### Forms
