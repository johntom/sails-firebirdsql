![image_squidhome@2x.png](http://i.imgur.com/RIvu9.png)

# FirebirdSQL Sails/Waterline Adapter

[![Build Status](https://travis-ci.org/balderdashy/sails-firebirdsql.png?branch=master)](https://travis-ci.org/balderdashy/sails-firebirdsql) [![NPM version](https://badge.fury.io/js/sails-firebirdsql.png)](http://badge.fury.io/js/sails-firebirdsql) [![Dependency Status](https://gemnasium.com/balderdashy/sails-firebirdsql.png)](https://gemnasium.com/balderdashy/sails-firebirdsql)

A [Waterline](https://github.com/balderdashy/waterline) adapter for FirebirdSQL. May be used in a [Sails](https://github.com/balderdashy/sails) app or anything using Waterline for the ORM.

## Install

Install is through NPM.

```bash
$ npm install sails-firebirdsql
```

## Configuration

The following config options are available along with their default values:

```javascript
config: {
  database: '/path/to/databaseName',
  host: 'localhost',
  user: 'SYSDBA',
  password: 'masterkey',
  port: 3050
};
```
Alternatively, you can supply the connection information in URL format:
```javascript
config: {
  url: 'firebird://username:password@hostname:port/database'
};
```

## Testing

Test are written with mocha. Integration tests are handled by the [waterline-adapter-tests](https://github.com/balderdashy/waterline-adapter-tests) project, which tests adapter methods against the latest Waterline API.

To run tests:

```bash
$ npm test
```

## About Waterline

Waterline is a new kind of storage and retrieval engine.  It provides a uniform API for accessing stuff from different kinds of databases, protocols, and 3rd party APIs.  That means you write the same code to get users, whether they live in mySQL, LDAP, MongoDB, or Facebook.

To learn more visit the project on GitHub at [Waterline](https://github.com/balderdashy/waterline).
