[![npm](https://img.shields.io/npm/v/kronos-message.svg)](https://www.npmjs.com/package/kronos-message)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/Kronos-Integration/kronos-message)
[![Build Status](https://secure.travis-ci.org/Kronos-Integration/kronos-message.png)](http://travis-ci.org/Kronos-Integration/kronos-message)
[![bithound](https://www.bithound.io/github/Kronos-Integration/kronos-message/badges/score.svg)](https://www.bithound.io/github/Kronos-Integration/kronos-message)
[![codecov.io](http://codecov.io/github/Kronos-Integration/kronos-message/coverage.svg?branch=master)](http://codecov.io/github/Kronos-Integration/kronos-message?branch=master)
[![Coverage Status](https://coveralls.io/repos/Kronos-Integration/kronos-message/badge.svg)](https://coveralls.io/r/Kronos-Integration/kronos-message)
[![Code Climate](https://codeclimate.com/github/Kronos-Integration/kronos-message/badges/gpa.svg)](https://codeclimate.com/github/Kronos-Integration/kronos-message)
[![Known Vulnerabilities](https://snyk.io/test/github/Kronos-Integration/kronos-message/badge.svg)](https://snyk.io/test/github/Kronos-Integration/kronos-message)
[![GitHub Issues](https://img.shields.io/github/issues/Kronos-Integration/kronos-message.svg?style=flat-square)](https://github.com/Kronos-Integration/kronos-message/issues)
[![Stories in Ready](https://badge.waffle.io/Kronos-Integration/kronos-message.svg?label=ready&title=Ready)](http://waffle.io/Kronos-Integration/kronos-message)
[![Dependency Status](https://david-dm.org/Kronos-Integration/kronos-message.svg)](https://david-dm.org/Kronos-Integration/kronos-message)
[![devDependency Status](https://david-dm.org/Kronos-Integration/kronos-message/dev-status.svg)](https://david-dm.org/Kronos-Integration/kronos-message#info=devDependencies)
[![docs](http://inch-ci.org/github/Kronos-Integration/kronos-message.svg?branch=master)](http://inch-ci.org/github/Kronos-Integration/kronos-message)
[![downloads](http://img.shields.io/npm/dm/kronos-message.svg?style=flat-square)](https://npmjs.org/package/kronos-message)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

kronos-message
=====
The message object is the 'data' object which will be send from step to step

# API Reference

* <a name="createMessage"></a>

## createMessage(newData, oldRequestMessage)
Creates a new request message structure. It will merge the new data into a copy of the old request.
Only thf fields 'info' and 'hops' will be copied

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| newData | <code>object</code> | This json is new generated data by the step. It has the follwing structure. 	                       newData : {                           "info" : {},                           "payload" :                         } |
| oldRequestMessage | <code>object</code> | The request message this step has received |


* <a name="addHop"></a>

## addHop(message, stepName, stepType, endpoint)
Adds a new way point to the message

**Kind**: global function  

| Param | Type | Description |
| --- | --- | --- |
| message | <code>object</code> | The message to add the new hop |
| stepName | <code>string</code> | The name of the current step which issues this way point |
| stepType | <code>string</code> | The typeName of the step |
| endpoint | <code>string</code> | The name of endpoint the message is routed through |


* * *

install
=======

With [npm](http://npmjs.org) do:

```shell
npm install kronos-message
```

license
=======

BSD-2-Clause
