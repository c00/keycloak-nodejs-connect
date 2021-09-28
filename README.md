# Keycloak Node.js Adapter without Issuer Check

## No issuer check

The only change between this fork and the original is the removal of the issuer check. If your local url for the auth server is different than the one your clients use, the issuer check will fail and tokens will not be verified.

While this is probably super useful and important and all that noise, there's also tons of requests on the internet requesting for some option to deal with different urls (all met with silence).

The plugin still uses the auth url from the settings to fetch the public keys, so I don't see a way in which this can be abused.

Having said that, don't use this unless you understand the risks.


[![Dependency Status](https://img.shields.io/david/keycloak/keycloak-nodejs-connect.svg?style=flat-square)](https://david-dm.org/keycloak/keycloak-nodejs-connect)
[![Coverage Status](https://coveralls.io/repos/github/keycloak/keycloak-nodejs-connect/badge.svg?branch=master)](https://coveralls.io/github/keycloak/keycloak-nodejs-connect?branch=master)

Keycloak is an Open Source Identity and Access Management solution for modern Applications and Services.

This repository contains the source code for the Keycloak Node.js adapter. This module makes it simple to implement a Node.js Connect-friendly
application that uses Keycloak for its authentication and authorization needs. 

## Help and Documentation

* [Documentation](https://www.keycloak.org/documentation.html)
* [User Mailing List](https://groups.google.com/d/forum/keycloak-user) - Mailing list for help and general questions about Keycloak
* [JIRA](https://issues.jboss.org/projects/KEYCLOAK) - Issue tracker for bugs and feature requests

## Reporting Security Vulnerabilities

If you've found a security vulnerability, please look at the [instructions on how to properly report it](http://www.keycloak.org/security.html)

## Reporting an issue

If you believe you have discovered a defect in the Node.js adapter please open an issue in our [Issue Tracker](https://issues.jboss.org/projects/KEYCLOAK).
Please remember to provide a good summary, description as well as steps to reproduce the issue.

## Getting started

To run Node.js adapter examples please try one of our [quickstarts](https://github.com/keycloak/keycloak-quickstarts.git).

For more details refer to the [Keycloak Documentation](https://www.keycloak.org/documentation.html).

### Writing Tests

To write tests refer to the [writing tests](docs/tests-development.md) guide.

## Contributing

Before contributing to Node.js adapter please read our [contributing guidelines](CONTRIBUTING.md).

## Other Keycloak Projects

* [Keycloak](https://github.com/keycloak/keycloak) - Keycloak Server and Java adapters
* [Keycloak Documentation](https://github.com/keycloak/keycloak-documentation) - Documentation for Keycloak
* [Keycloak QuickStarts](https://github.com/keycloak/keycloak-quickstarts) - QuickStarts for getting started with Keycloak
* [Keycloak Docker](https://github.com/jboss-dockerfiles/keycloak) - Docker images for Keycloak
* [Keycloak Node.js Admin Client](https://github.com/keycloak/keycloak-nodejs-admin-client) - Node.js library for Keycloak Admin REST API

## License

* [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)
