# api documentation for  [node-notifier (v5.1.2)](https://github.com/mikaelbr/node-notifier#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-notifier.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-notifier)
#### A Node.js module for sending notifications on native Mac, Windows (post and pre 8) and Linux (or Growl as fallback)

[![NPM](https://nodei.co/npm/node-notifier.png?downloads=true)](https://www.npmjs.com/package/node-notifier)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-notifier/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-notifier_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-notifier/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-node-notifier/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Mikael Brevik"
    },
    "bugs": {
        "url": "https://github.com/mikaelbr/node-notifier/issues"
    },
    "dependencies": {
        "growly": "^1.3.0",
        "semver": "^5.3.0",
        "shellwords": "^0.1.0",
        "which": "^1.2.12"
    },
    "description": "A Node.js module for sending notifications on native Mac, Windows (post and pre 8) and Linux (or Growl as fallback)",
    "devDependencies": {
        "eslint": "^3.13.1",
        "eslint-config-semistandard": "^7.0.0",
        "eslint-config-standard": "^6.2.1",
        "eslint-plugin-promise": "^3.4.0",
        "eslint-plugin-standard": "^2.0.1",
        "jest": "^18.1.0"
    },
    "directories": {
        "example": "example",
        "test": "test"
    },
    "dist": {
        "shasum": "2fa9e12605fa10009d44549d6fcd8a63dde0e4ff",
        "tarball": "https://registry.npmjs.org/node-notifier/-/node-notifier-5.1.2.tgz"
    },
    "gitHead": "0b75bc5f6099bd5aeaac3e6c34e3a7e75edaba7e",
    "homepage": "https://github.com/mikaelbr/node-notifier#readme",
    "jest": {
        "testRegex": "/test/[^_]*.js",
        "testEnvironment": "node",
        "setupTestFrameworkScriptFile": "./test/_test-matchers.js"
    },
    "keywords": [
        "notification center",
        "mac os x 10.8",
        "notify",
        "terminal-notifier",
        "notify-send",
        "growl",
        "windows 8 notification",
        "toaster",
        "notification"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mikaelb",
            "email": "mikaelbre@gmail.com"
        }
    ],
    "name": "node-notifier",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/mikaelbr/node-notifier.git"
    },
    "scripts": {
        "example": "node ./example/message.js",
        "example:mac": "node ./example/advanced.js",
        "example:mac:input": "node ./example/macInput.js",
        "example:windows": "node ./example/toaster.js",
        "lint": "eslint example/*.js lib/*.js notifiers/*.js test/**/*.js index.js",
        "pretest": "npm run lint",
        "test": "jest"
    },
    "version": "5.1.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-notifier](#apidoc.module.node-notifier)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>Growl (options)](#apidoc.element.node-notifier.Growl)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>Notification (options)](#apidoc.element.node-notifier.Notification)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>NotificationCenter (options)](#apidoc.element.node-notifier.NotificationCenter)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>NotifySend (options)](#apidoc.element.node-notifier.NotifySend)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>WindowsBalloon (options)](#apidoc.element.node-notifier.WindowsBalloon)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>WindowsToaster (options)](#apidoc.element.node-notifier.WindowsToaster)
1.  number <span class="apidocSignatureSpan">node-notifier.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">node-notifier.</span>Growl.prototype
1.  object <span class="apidocSignatureSpan">node-notifier.</span>Notification.prototype
1.  object <span class="apidocSignatureSpan">node-notifier.</span>NotificationCenter.prototype
1.  object <span class="apidocSignatureSpan">node-notifier.</span>WindowsBalloon.prototype
1.  object <span class="apidocSignatureSpan">node-notifier.</span>WindowsToaster.prototype
1.  object <span class="apidocSignatureSpan">node-notifier.</span>_events
1.  object <span class="apidocSignatureSpan">node-notifier.</span>domain
1.  object <span class="apidocSignatureSpan">node-notifier.</span>options
1.  object <span class="apidocSignatureSpan">node-notifier.</span>utils

#### [module node-notifier.Growl](#apidoc.module.node-notifier.Growl)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>Growl (options)](#apidoc.element.node-notifier.Growl.Growl)
1.  [function <span class="apidocSignatureSpan">node-notifier.Growl.</span>super_ ()](#apidoc.element.node-notifier.Growl.super_)

#### [module node-notifier.Growl.prototype](#apidoc.module.node-notifier.Growl.prototype)
1.  [function <span class="apidocSignatureSpan">node-notifier.Growl.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.Growl.prototype.notify)

#### [module node-notifier.Notification](#apidoc.module.node-notifier.Notification)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>Notification (options)](#apidoc.element.node-notifier.Notification.Notification)
1.  [function <span class="apidocSignatureSpan">node-notifier.Notification.</span>super_ ()](#apidoc.element.node-notifier.Notification.super_)

#### [module node-notifier.Notification.prototype](#apidoc.module.node-notifier.Notification.prototype)
1.  [function <span class="apidocSignatureSpan">node-notifier.Notification.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.Notification.prototype.notify)

#### [module node-notifier.NotificationCenter](#apidoc.module.node-notifier.NotificationCenter)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>NotificationCenter (options)](#apidoc.element.node-notifier.NotificationCenter.NotificationCenter)
1.  [function <span class="apidocSignatureSpan">node-notifier.NotificationCenter.</span>super_ ()](#apidoc.element.node-notifier.NotificationCenter.super_)

#### [module node-notifier.NotificationCenter.prototype](#apidoc.module.node-notifier.NotificationCenter.prototype)
1.  [function <span class="apidocSignatureSpan">node-notifier.NotificationCenter.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.NotificationCenter.prototype.notify)

#### [module node-notifier.WindowsBalloon](#apidoc.module.node-notifier.WindowsBalloon)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>WindowsBalloon (options)](#apidoc.element.node-notifier.WindowsBalloon.WindowsBalloon)
1.  [function <span class="apidocSignatureSpan">node-notifier.WindowsBalloon.</span>super_ ()](#apidoc.element.node-notifier.WindowsBalloon.super_)

#### [module node-notifier.WindowsBalloon.prototype](#apidoc.module.node-notifier.WindowsBalloon.prototype)
1.  [function <span class="apidocSignatureSpan">node-notifier.WindowsBalloon.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.WindowsBalloon.prototype.notify)

#### [module node-notifier.WindowsToaster](#apidoc.module.node-notifier.WindowsToaster)
1.  [function <span class="apidocSignatureSpan">node-notifier.</span>WindowsToaster (options)](#apidoc.element.node-notifier.WindowsToaster.WindowsToaster)
1.  [function <span class="apidocSignatureSpan">node-notifier.WindowsToaster.</span>super_ ()](#apidoc.element.node-notifier.WindowsToaster.super_)

#### [module node-notifier.WindowsToaster.prototype](#apidoc.module.node-notifier.WindowsToaster.prototype)
1.  [function <span class="apidocSignatureSpan">node-notifier.WindowsToaster.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.WindowsToaster.prototype.notify)

#### [module node-notifier.utils](#apidoc.module.node-notifier.utils)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>actionJackerDecorator (emitter, options, fn, mapper)](#apidoc.element.node-notifier.utils.actionJackerDecorator)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>clone (obj)](#apidoc.element.node-notifier.utils.clone)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>command (notifier, options, cb)](#apidoc.element.node-notifier.utils.command)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>constructArgumentList (options, extra)](#apidoc.element.node-notifier.utils.constructArgumentList)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>fileCommand (notifier, options, cb)](#apidoc.element.node-notifier.utils.fileCommand)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>fileCommandJson (notifier, options, cb)](#apidoc.element.node-notifier.utils.fileCommandJson)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>immediateFileCommand (notifier, options, cb)](#apidoc.element.node-notifier.utils.immediateFileCommand)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>isLessThanWin8 ()](#apidoc.element.node-notifier.utils.isLessThanWin8)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>isMac ()](#apidoc.element.node-notifier.utils.isMac)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>isMountainLion ()](#apidoc.element.node-notifier.utils.isMountainLion)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>isWin8 ()](#apidoc.element.node-notifier.utils.isWin8)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToGrowl (options)](#apidoc.element.node-notifier.utils.mapToGrowl)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToMac (options)](#apidoc.element.node-notifier.utils.mapToMac)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToNotifu (options)](#apidoc.element.node-notifier.utils.mapToNotifu)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToNotifySend (options)](#apidoc.element.node-notifier.utils.mapToNotifySend)
1.  [function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToWin8 (options)](#apidoc.element.node-notifier.utils.mapToWin8)



# <a name="apidoc.module.node-notifier"></a>[module node-notifier](#apidoc.module.node-notifier)

#### <a name="apidoc.element.node-notifier.Growl"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>Growl (options)](#apidoc.element.node-notifier.Growl)
- description and source-code
```javascript
function Growl(options) {
  options = utils.clone(options || {});
  if (!(this instanceof Growl)) {
    return new Growl(options);
  }

  growly.appname = options.name || 'Node';
  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...
'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents

* [Notification Center documentation](#usage-notificationcenter)
* [Windows Toaster documentation](#usage-windowstoaster)
* [Windows Balloon documentation](#usage-windowsballoon)
...
```

#### <a name="apidoc.element.node-notifier.Notification"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>Notification (options)](#apidoc.element.node-notifier.Notification)
- description and source-code
```javascript
function NotifySend(options) {
  options = utils.clone(options || {});
  if (!(this instanceof NotifySend)) {
    return new NotifySend(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.NotificationCenter"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>NotificationCenter (options)](#apidoc.element.node-notifier.NotificationCenter)
- description and source-code
```javascript
function NotificationCenter(options) {
  options = utils.clone(options || {});
  if (!(this instanceof NotificationCenter)) {
    return new NotificationCenter(options);
  }
  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...

Or if you are using several (or you are lazy):
(note: technically, this takes longer to require)

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents
...
```

#### <a name="apidoc.element.node-notifier.NotifySend"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>NotifySend (options)](#apidoc.element.node-notifier.NotifySend)
- description and source-code
```javascript
function NotifySend(options) {
  options = utils.clone(options || {});
  if (!(this instanceof NotifySend)) {
    return new NotifySend(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...
Or if you are using several (or you are lazy):
(note: technically, this takes longer to require)

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents
...
```

#### <a name="apidoc.element.node-notifier.WindowsBalloon"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>WindowsBalloon (options)](#apidoc.element.node-notifier.WindowsBalloon)
- description and source-code
```javascript
function WindowsBalloon(options) {
  options = utils.clone(options || {});
  if (!(this instanceof WindowsBalloon)) {
    return new WindowsBalloon(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents

* [Notification Center documentation](#usage-notificationcenter)
* [Windows Toaster documentation](#usage-windowstoaster)
...
```

#### <a name="apidoc.element.node-notifier.WindowsToaster"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>WindowsToaster (options)](#apidoc.element.node-notifier.WindowsToaster)
- description and source-code
```javascript
function WindowsToaster(options) {
  options = utils.clone(options || {});
  if (!(this instanceof WindowsToaster)) {
    return new WindowsToaster(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...
(note: technically, this takes longer to require)

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents

* [Notification Center documentation](#usage-notificationcenter)
...
```



# <a name="apidoc.module.node-notifier.Growl"></a>[module node-notifier.Growl](#apidoc.module.node-notifier.Growl)

#### <a name="apidoc.element.node-notifier.Growl.Growl"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>Growl (options)](#apidoc.element.node-notifier.Growl.Growl)
- description and source-code
```javascript
function Growl(options) {
  options = utils.clone(options || {});
  if (!(this instanceof Growl)) {
    return new Growl(options);
  }

  growly.appname = options.name || 'Node';
  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...
'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents

* [Notification Center documentation](#usage-notificationcenter)
* [Windows Toaster documentation](#usage-windowstoaster)
* [Windows Balloon documentation](#usage-windowsballoon)
...
```

#### <a name="apidoc.element.node-notifier.Growl.super_"></a>[function <span class="apidocSignatureSpan">node-notifier.Growl.</span>super_ ()](#apidoc.element.node-notifier.Growl.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-notifier.Growl.prototype"></a>[module node-notifier.Growl.prototype](#apidoc.module.node-notifier.Growl.prototype)

#### <a name="apidoc.element.node-notifier.Growl.prototype.notify"></a>[function <span class="apidocSignatureSpan">node-notifier.Growl.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.Growl.prototype.notify)
- description and source-code
```javascript
notify = function (options, callback) {
  growly.setHost(this.options.host, this.options.port);
  options = utils.clone(options || {});

  if (typeof options === 'string') {
    options = { title: 'node-notifier', message: options };
  }

  callback = utils.actionJackerDecorator(this, options, callback, function(
    data
  ) {
    if (data === 'click') {
      return 'click';
    }
    if (data === 'timedout') {
      return 'timeout';
    }
    return false;
  });

  options = utils.mapToGrowl(options);

  if (!options.message) {
    callback(new Error('Message is required.'));
    return this;
  }

  options.title = options.title || 'Node Notification:';

  if (hasGrowl || !!options.wait) {
    var localCallback = options.wait ? callback : noop;
    growly.notify(options.message, options, localCallback);
    if (!options.wait) callback();
    return this;
  }

  checkGrowl(growly, function(didHaveGrowl) {
    hasGrowl = didHaveGrowl;
    if (!didHaveGrowl) return callback(new Error(errorMessageNotFound));
    growly.notify(options.message, options);
    callback();
  });
  return this;
}
```
- example usage
```shell
...
## Quick Usage

Show a native notification on macOS, Windows, Linux:

'''javascript
const notifier = require('node-notifier');
// String
notifier.notify('Message');

// Object
notifier.notify({
  'title': 'My notification',
  'message': 'Hello, there!'
});
'''
...
```



# <a name="apidoc.module.node-notifier.Notification"></a>[module node-notifier.Notification](#apidoc.module.node-notifier.Notification)

#### <a name="apidoc.element.node-notifier.Notification.Notification"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>Notification (options)](#apidoc.element.node-notifier.Notification.Notification)
- description and source-code
```javascript
function NotifySend(options) {
  options = utils.clone(options || {});
  if (!(this instanceof NotifySend)) {
    return new NotifySend(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.Notification.super_"></a>[function <span class="apidocSignatureSpan">node-notifier.Notification.</span>super_ ()](#apidoc.element.node-notifier.Notification.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-notifier.Notification.prototype"></a>[module node-notifier.Notification.prototype](#apidoc.module.node-notifier.Notification.prototype)

#### <a name="apidoc.element.node-notifier.Notification.prototype.notify"></a>[function <span class="apidocSignatureSpan">node-notifier.Notification.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.Notification.prototype.notify)
- description and source-code
```javascript
notify = function (options, callback) {
  options = utils.clone(options || {});
  callback = callback || noop;

  if (typeof callback !== 'function') {
    throw new TypeError(
      'The second argument must be a function callback. You have passed ' +
        typeof callback
    );
  }

  if (typeof options === 'string') {
    options = { title: 'node-notifier', message: options };
  }

  if (!options.message) {
    callback(new Error('Message is required.'));
    return this;
  }

  if (os.type() !== 'Linux' && !os.type().match(/BSD$/)) {
    callback(new Error('Only supported on Linux and *BSD systems'));
    return this;
  }

  if (hasNotifier === false) {
    callback(new Error('notify-send must be installed on the system.'));
    return this;
  }

  if (hasNotifier || !!this.options.suppressOsdCheck) {
    doNotification(options, callback);
    return this;
  }

  try {
    hasNotifier = !!which.sync(notifier);
    doNotification(options, callback);
  } catch (err) {
    hasNotifier = false;
    return callback(err);
  }

  return this;
}
```
- example usage
```shell
...
## Quick Usage

Show a native notification on macOS, Windows, Linux:

'''javascript
const notifier = require('node-notifier');
// String
notifier.notify('Message');

// Object
notifier.notify({
  'title': 'My notification',
  'message': 'Hello, there!'
});
'''
...
```



# <a name="apidoc.module.node-notifier.NotificationCenter"></a>[module node-notifier.NotificationCenter](#apidoc.module.node-notifier.NotificationCenter)

#### <a name="apidoc.element.node-notifier.NotificationCenter.NotificationCenter"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>NotificationCenter (options)](#apidoc.element.node-notifier.NotificationCenter.NotificationCenter)
- description and source-code
```javascript
function NotificationCenter(options) {
  options = utils.clone(options || {});
  if (!(this instanceof NotificationCenter)) {
    return new NotificationCenter(options);
  }
  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...

Or if you are using several (or you are lazy):
(note: technically, this takes longer to require)

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents
...
```

#### <a name="apidoc.element.node-notifier.NotificationCenter.super_"></a>[function <span class="apidocSignatureSpan">node-notifier.NotificationCenter.</span>super_ ()](#apidoc.element.node-notifier.NotificationCenter.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-notifier.NotificationCenter.prototype"></a>[module node-notifier.NotificationCenter.prototype](#apidoc.module.node-notifier.NotificationCenter.prototype)

#### <a name="apidoc.element.node-notifier.NotificationCenter.prototype.notify"></a>[function <span class="apidocSignatureSpan">node-notifier.NotificationCenter.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.NotificationCenter.prototype.notify)
- description and source-code
```javascript
notify = function (options, callback) {
  var fallbackNotifier;
  var id = identificator();
  options = utils.clone(options || {});
  activeId = id;

  if (typeof options === 'string') {
    options = { title: 'node-notifier', message: options };
  }
  var timeout;

  callback = callback || noop;

  if (typeof callback !== 'function') {
    throw new TypeError(
      'The second argument must be a function callback. You have passed ' +
        typeof fn
    );
  }

  var actionJackedCallback = utils.actionJackerDecorator(
    this,
    options,
    function() {
      clearTimeout(timeout);
      callback.apply(null, arguments);
    },
    function(data) {
      if (activeId !== id) return false;

      if (data === 'activate') {
        return 'click';
      }
      if (data === 'timeout') {
        return 'timeout';
      }
      if (data === 'replied') {
        return 'replied';
      }
      return false;
    }
  );

  options = utils.mapToMac(options);

  if (!options.message && !options.group && !options.list && !options.remove) {
    callback(new Error('Message, group, remove or list property is required.'));
    return this;
  }

  var argsList = utils.constructArgumentList(options);
  if (utils.isMountainLion()) {
    var cp = utils.fileCommandJson(
      this.options.customPath || notifier,
      argsList,
      actionJackedCallback
    );
    // Redundancy fallback to prevent memory leak
    timeout = setTimeout(
      function() {
        cp.kill('SIGTERM');
      },
      FAILSAFE_TIMEOUT
    );

    return this;
  }

  if (fallbackNotifier || !!this.options.withFallback) {
    fallbackNotifier = fallbackNotifier || new Growl(this.options);
    return fallbackNotifier.notify(options, callback);
  }

  callback(new Error(errorMessageOsX));
  return this;
}
```
- example usage
```shell
...
## Quick Usage

Show a native notification on macOS, Windows, Linux:

'''javascript
const notifier = require('node-notifier');
// String
notifier.notify('Message');

// Object
notifier.notify({
  'title': 'My notification',
  'message': 'Hello, there!'
});
'''
...
```



# <a name="apidoc.module.node-notifier.WindowsBalloon"></a>[module node-notifier.WindowsBalloon](#apidoc.module.node-notifier.WindowsBalloon)

#### <a name="apidoc.element.node-notifier.WindowsBalloon.WindowsBalloon"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>WindowsBalloon (options)](#apidoc.element.node-notifier.WindowsBalloon.WindowsBalloon)
- description and source-code
```javascript
function WindowsBalloon(options) {
  options = utils.clone(options || {});
  if (!(this instanceof WindowsBalloon)) {
    return new WindowsBalloon(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents

* [Notification Center documentation](#usage-notificationcenter)
* [Windows Toaster documentation](#usage-windowstoaster)
...
```

#### <a name="apidoc.element.node-notifier.WindowsBalloon.super_"></a>[function <span class="apidocSignatureSpan">node-notifier.WindowsBalloon.</span>super_ ()](#apidoc.element.node-notifier.WindowsBalloon.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-notifier.WindowsBalloon.prototype"></a>[module node-notifier.WindowsBalloon.prototype](#apidoc.module.node-notifier.WindowsBalloon.prototype)

#### <a name="apidoc.element.node-notifier.WindowsBalloon.prototype.notify"></a>[function <span class="apidocSignatureSpan">node-notifier.WindowsBalloon.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.WindowsBalloon.prototype.notify)
- description and source-code
```javascript
notify = function (options, callback) {
  var fallback;
  var notifierOptions = this.options;
  options = utils.clone(options || {});
  callback = callback || noop;

  if (typeof options === 'string') {
    options = { title: 'node-notifier', message: options };
  }

  var actionJackedCallback = utils.actionJackerDecorator(
    this,
    options,
    callback,
    function(data) {
      if (data === 'activate') {
        return 'click';
      }
      if (data === 'timeout') {
        return 'timeout';
      }
      return false;
    }
  );

  if (!!this.options.withFallback && utils.isWin8()) {
    fallback = fallback || new Toaster(notifierOptions);
    return fallback.notify(options, callback);
  }

  if (
    !!this.options.withFallback &&
      (!utils.isLessThanWin8() || hasGrowl === true)
  ) {
    fallback = fallback || new Growl(notifierOptions);
    return fallback.notify(options, callback);
  }

  if (!this.options.withFallback || hasGrowl === false) {
    doNotification(options, notifierOptions, actionJackedCallback);
    return this;
  }

  checkGrowl(notifierOptions, function(hasGrowlResult) {
    hasGrowl = hasGrowlResult;

    if (hasGrowl) {
      fallback = fallback || new Growl(notifierOptions);
      return fallback.notify(options, callback);
    }

    doNotification(options, notifierOptions, actionJackedCallback);
  });

  return this;
}
```
- example usage
```shell
...
## Quick Usage

Show a native notification on macOS, Windows, Linux:

'''javascript
const notifier = require('node-notifier');
// String
notifier.notify('Message');

// Object
notifier.notify({
  'title': 'My notification',
  'message': 'Hello, there!'
});
'''
...
```



# <a name="apidoc.module.node-notifier.WindowsToaster"></a>[module node-notifier.WindowsToaster](#apidoc.module.node-notifier.WindowsToaster)

#### <a name="apidoc.element.node-notifier.WindowsToaster.WindowsToaster"></a>[function <span class="apidocSignatureSpan">node-notifier.</span>WindowsToaster (options)](#apidoc.element.node-notifier.WindowsToaster.WindowsToaster)
- description and source-code
```javascript
function WindowsToaster(options) {
  options = utils.clone(options || {});
  if (!(this instanceof WindowsToaster)) {
    return new WindowsToaster(options);
  }

  this.options = options;

  EventEmitter.call(this);
}
```
- example usage
```shell
...
(note: technically, this takes longer to require)

'''javascript
const nn = require('node-notifier');

new nn.NotificationCenter(options).notify();
new nn.NotifySend(options).notify();
new nn.WindowsToaster(options).notify(options);
new nn.WindowsBalloon(options).notify(options);
new nn.Growl(options).notify(options);
'''

## Contents

* [Notification Center documentation](#usage-notificationcenter)
...
```

#### <a name="apidoc.element.node-notifier.WindowsToaster.super_"></a>[function <span class="apidocSignatureSpan">node-notifier.WindowsToaster.</span>super_ ()](#apidoc.element.node-notifier.WindowsToaster.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-notifier.WindowsToaster.prototype"></a>[module node-notifier.WindowsToaster.prototype](#apidoc.module.node-notifier.WindowsToaster.prototype)

#### <a name="apidoc.element.node-notifier.WindowsToaster.prototype.notify"></a>[function <span class="apidocSignatureSpan">node-notifier.WindowsToaster.prototype.</span>notify (options, callback)](#apidoc.element.node-notifier.WindowsToaster.prototype.notify)
- description and source-code
```javascript
notify = function (options, callback) {
  options = utils.clone(options || {});
  callback = callback || noop;

  if (typeof options === 'string') {
    options = { title: 'node-notifier', message: options };
  }

  if (typeof callback !== 'function') {
    throw new TypeError(
      'The second argument must be a function callback. You have passed ' +
        typeof fn
    );
  }

  var actionJackedCallback = utils.actionJackerDecorator(
    this,
    options,
    function cb(err, data) {
      // Needs to filter out timeout. Not an actual error.
      if (err && hasText(data, timeoutMessage)) {
        return callback(null, data);
      }
      callback(err, data);
    },
    function mapper(data) {
      if (hasText(data, successMessage)) {
        return 'click';
      }
      if (hasText(data, timeoutMessage)) {
        return 'timeout';
      }
      return false;
    }
  );

  options.title = options.title || 'Node Notification:';
  if (
    typeof options.message === 'undefined' &&
      typeof options.close === 'undefined'
  ) {
    callback(new Error('Message or ID to close is required.'));
    return this;
  }

  if (!utils.isWin8() && !!this.options.withFallback) {
    fallback = fallback || new Balloon(this.options);
    return fallback.notify(options, callback);
  }

  options = utils.mapToWin8(options);
  var argsList = utils.constructArgumentList(options, {
    explicitTrue: true,
    wrapper: '',
    keepNewlines: true,
    noEscape: true
  });
  utils.fileCommand(
    this.options.customPath || notifier,
    argsList,
    actionJackedCallback
  );
  return this;
}
```
- example usage
```shell
...
## Quick Usage

Show a native notification on macOS, Windows, Linux:

'''javascript
const notifier = require('node-notifier');
// String
notifier.notify('Message');

// Object
notifier.notify({
  'title': 'My notification',
  'message': 'Hello, there!'
});
'''
...
```



# <a name="apidoc.module.node-notifier.utils"></a>[module node-notifier.utils](#apidoc.module.node-notifier.utils)

#### <a name="apidoc.element.node-notifier.utils.actionJackerDecorator"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>actionJackerDecorator (emitter, options, fn, mapper)](#apidoc.element.node-notifier.utils.actionJackerDecorator)
- description and source-code
```javascript
actionJackerDecorator = function (emitter, options, fn, mapper) {
  options = clone(options);
  fn = fn || noop;

  if (typeof fn !== 'function') {
    throw new TypeError(
      'The second argument must be a function callback. You have passed ' +
        typeof fn
    );
  }

  return function(err, data) {
    var resultantData = data;
    var metadata = {};
    // Allow for extra data if resultantData is an object
    if (resultantData && typeof resultantData === 'object') {
      metadata = resultantData;
      resultantData = resultantData.activationType;
    }

    // Sanitize the data
    if (resultantData) {
      resultantData = resultantData.toLowerCase().trim();
      if (resultantData.match(/^activate|clicked$/)) {
        resultantData = 'activate';
      }
    }

    fn.apply(emitter, [err, resultantData, metadata]);
    if (!mapper || !resultantData) return;

    var key = mapper(resultantData);
    if (!key) return;
    emitter.emit(key, emitter, options, metadata);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.clone"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>clone (obj)](#apidoc.element.node-notifier.utils.clone)
- description and source-code
```javascript
function clone(obj) {
  return JSON.parse(JSON.stringify(obj));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.command"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>command (notifier, options, cb)](#apidoc.element.node-notifier.utils.command)
- description and source-code
```javascript
command = function (notifier, options, cb) {
  notifier = shellwords.escape(notifier);
  if (process.env.DEBUG) {
    console.info('node-notifier debug info (command):');
    console.info('[notifier path]', notifier);
    console.info('[notifier options]', options.join(' '));
  }

  return cp.exec(
    notifier + ' ' + options.join(' '),
    function(error, stdout, stderr) {
      if (error) return cb(error);
      cb(stderr, stdout);
    }
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.constructArgumentList"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>constructArgumentList (options, extra)](#apidoc.element.node-notifier.utils.constructArgumentList)
- description and source-code
```javascript
constructArgumentList = function (options, extra) {
  var args = [];
  extra = extra || {};

  // Massive ugly setup. Default args
  var initial = extra.initial || [];
  var keyExtra = extra.keyExtra || '';
  var allowedArguments = extra.allowedArguments || [];
  var noEscape = extra.noEscape !== void 0;
  var checkForAllowed = extra.allowedArguments !== void 0;
  var explicitTrue = !!extra.explicitTrue;
  var keepNewlines = !!extra.keepNewlines;
  var wrapper = extra.wrapper === void 0 ? '"' : extra.wrapper;

  var escapeFn = function(arg) {
    if (isArray(arg)) {
      return removeNewLines(arg.join(','));
    }

    if (!noEscape) {
      arg = escapeQuotes(arg);
    }
    if (typeof arg === 'string' && !keepNewlines) {
      arg = removeNewLines(arg);
    }
    return wrapper + arg + wrapper;
  };

  initial.forEach(function(val) {
    args.push(escapeFn(val));
  });
  for (var key in options) {
    if (
      options.hasOwnProperty(key) &&
      (!checkForAllowed || inArray(allowedArguments, key))
    ) {
      if (explicitTrue && options[key] === true) {
        args.push('-' + keyExtra + key);
      } else if (explicitTrue && options[key] === false) continue;
      else args.push('-' + keyExtra + key, escapeFn(options[key]));
    }
  }
  return args;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.fileCommand"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>fileCommand (notifier, options, cb)](#apidoc.element.node-notifier.utils.fileCommand)
- description and source-code
```javascript
fileCommand = function (notifier, options, cb) {
  if (process.env.DEBUG) {
    console.info('node-notifier debug info (fileCommand):');
    console.info('[notifier path]', notifier);
    console.info('[notifier options]', options.join(' '));
  }

  return cp.execFile(notifier, options, function(error, stdout, stderr) {
    if (error) return cb(error, stdout);
    cb(stderr, stdout);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.fileCommandJson"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>fileCommandJson (notifier, options, cb)](#apidoc.element.node-notifier.utils.fileCommandJson)
- description and source-code
```javascript
fileCommandJson = function (notifier, options, cb) {
  if (process.env.DEBUG) {
    console.info('node-notifier debug info (fileCommandJson):');
    console.info('[notifier path]', notifier);
    console.info('[notifier options]', options.join(' '));
  }
  return cp.execFile(notifier, options, function(error, stdout, stderr) {
    if (error) return cb(error, stdout);
    if (!stdout) return cb(error, {});

    try {
      var data = JSON.parse(stdout);
      cb(stderr, data);
    } catch (e) {
      cb(e, stdout);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.immediateFileCommand"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>immediateFileCommand (notifier, options, cb)](#apidoc.element.node-notifier.utils.immediateFileCommand)
- description and source-code
```javascript
immediateFileCommand = function (notifier, options, cb) {
  if (process.env.DEBUG) {
    console.info('node-notifier debug info (notifier):');
    console.info('[notifier path]', notifier);
  }

  notifierExists(notifier, function(exists) {
    if (!exists) {
      return cb(new Error('Notifier (' + notifier + ') not found on system.'));
    }
    cp.execFile(notifier, options);
    cb();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.isLessThanWin8"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>isLessThanWin8 ()](#apidoc.element.node-notifier.utils.isLessThanWin8)
- description and source-code
```javascript
isLessThanWin8 = function () {
  return os.type() === 'Windows_NT' &&
    semver.satisfies(garanteeSemverFormat(os.release()), '<6.2.9200');
}
```
- example usage
```shell
...
  module.exports.Notification = NotifySend;
  break;
case 'Darwin':
  module.exports = new NotificationCenter(options);
  module.exports.Notification = NotificationCenter;
  break;
case 'Windows_NT':
  if (utils.isLessThanWin8()) {
    module.exports = new WindowsBalloon(options);
    module.exports.Notification = WindowsBalloon;
  } else {
    module.exports = new WindowsToaster(options);
    module.exports.Notification = WindowsToaster;
  }
  break;
...
```

#### <a name="apidoc.element.node-notifier.utils.isMac"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>isMac ()](#apidoc.element.node-notifier.utils.isMac)
- description and source-code
```javascript
isMac = function () {
  return os.type() === 'Darwin';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.isMountainLion"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>isMountainLion ()](#apidoc.element.node-notifier.utils.isMountainLion)
- description and source-code
```javascript
isMountainLion = function () {
  return os.type() === 'Darwin' &&
    semver.satisfies(garanteeSemverFormat(os.release()), '>=12.0.0');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.isWin8"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>isWin8 ()](#apidoc.element.node-notifier.utils.isWin8)
- description and source-code
```javascript
isWin8 = function () {
  return os.type() === 'Windows_NT' &&
    semver.satisfies(garanteeSemverFormat(os.release()), '>=6.2.9200');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.mapToGrowl"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToGrowl (options)](#apidoc.element.node-notifier.utils.mapToGrowl)
- description and source-code
```javascript
mapToGrowl = function (options) {
  options = mapAppIcon(options);
  options = mapIconShorthand(options);
  options = mapText(options);

  if (options.icon && !Buffer.isBuffer(options.icon)) {
    try {
      options.icon = fs.readFileSync(options.icon);
    } catch (ex) {}
  }

  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.mapToMac"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToMac (options)](#apidoc.element.node-notifier.utils.mapToMac)
- description and source-code
```javascript
mapToMac = function (options) {
  options = mapIconShorthand(options);
  options = mapText(options);

  if (options.icon) {
    options.appIcon = options.icon;
    delete options.icon;
  }

  if (options.sound === true) {
    options.sound = 'Bottle';
  }

  if (options.sound === false) {
    delete options.sound;
  }

  if (options.sound && options.sound.indexOf('Notification.') === 0) {
    options.sound = 'Bottle';
  }

  if (options.wait === true) {
    if (!options.timeout) {
      options.timeout = 5;
    }
    delete options.wait;
  }

  options.json = true;
  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.mapToNotifu"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToNotifu (options)](#apidoc.element.node-notifier.utils.mapToNotifu)
- description and source-code
```javascript
mapToNotifu = function (options) {
  options = mapAppIcon(options);
  options = mapText(options);

  if (options.icon) {
    options.i = options.icon;
    delete options.icon;
  }

  if (options.message) {
    options.m = options.message;
    delete options.message;
  }

  if (options.title) {
    options.p = options.title;
    delete options.title;
  }

  if (options.time) {
    options.d = options.time;
    delete options.time;
  }

  if (options.q !== false) {
    options.q = true;
  } else {
    delete options.q;
  }

  if (options.quiet === false) {
    delete options.q;
    delete options.quiet;
  }

  if (options.sound) {
    delete options.q;
    delete options.sound;
  }

  if (options.t) {
    options.d = options.t;
    delete options.t;
  }

  if (options.type) {
    options.t = sanitizeNotifuTypeArgument(options.type);
    delete options.type;
  }

  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.mapToNotifySend"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToNotifySend (options)](#apidoc.element.node-notifier.utils.mapToNotifySend)
- description and source-code
```javascript
mapToNotifySend = function (options) {
  options = mapAppIcon(options);
  options = mapText(options);

  for (var key in options) {
    if (key === 'message' || key === 'title') continue;
    if (options.hasOwnProperty(key) && notifySendFlags[key] !== key) {
      options[notifySendFlags[key]] = options[key];
      delete options[key];
    }
  }

  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-notifier.utils.mapToWin8"></a>[function <span class="apidocSignatureSpan">node-notifier.utils.</span>mapToWin8 (options)](#apidoc.element.node-notifier.utils.mapToWin8)
- description and source-code
```javascript
mapToWin8 = function (options) {
  options = mapAppIcon(options);
  options = mapText(options);

  if (options.icon) {
    if (/^file:\/+/.test(options.icon)) {
      // should parse file protocol URL to path
      options.p = url
        .parse(options.icon)
        .pathname.replace(/^\/(\w:\/)/, '$1')
        .replace(/\//g, '\\');
    } else {
      options.p = options.icon;
    }
    delete options.icon;
  }

  if (options.message) {
    // Remove escape char to debug "HRESULT : 0xC00CE508" exception
    options.m = options.message.replace(/\x1b/g, '');
    delete options.message;
  }

  if (options.title) {
    options.t = options.title;
    delete options.title;
  }

  if (options.appName) {
    options.appID = options.appName;
    delete options.appName;
  } else {
    options.appID = ' ';
  }

  if (typeof options.appID === 'undefined') {
    options.appID = ' ';
  }

  if (typeof options.remove !== 'undefined') {
    options.close = options.remove;
    delete options.remove;
  }

  if (options.quiet || options.silent) {
    options.silent = options.quiet || options.silent;
    delete options.quiet;
  }

  if (typeof options.sound !== 'undefined') {
    options.s = options.sound;
    delete options.sound;
  }

  if (options.s === false) {
    options.silent = true;
    delete options.s;
  }

  // Silent takes precedence. Remove sound.
  if (options.s && options.silent) {
    delete options.s;
  }

  if (options.s === true) {
    options.s = toasterDefaultSound;
  }

  if (options.s && options.s.indexOf(toasterSoundPrefix) !== 0) {
    options.s = toasterDefaultSound;
  }

  if (options.wait) {
    options.w = options.wait;
    delete options.wait;
  }

  for (var key in options) {
    // Check if is allowed. If not, delete!
    if (
      options.hasOwnProperty(key) && allowedToasterFlags.indexOf(key) === -1
    ) {
      delete options[key];
    }
  }

  return options;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
