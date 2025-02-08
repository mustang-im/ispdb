# ISPDB - Database of mail, calendar, contacts, chat and file server configuration

The purpose is for end users to seamlessly set up their email accounts and chat, file, calendar and contacts accounts, by entering only their email address and password or authentication.

## Scope

This database contains the configuration for almost all large ISPs in the world. Most ISPs with a userbase of more than 0.1% are in this database.

This ISPDB is - as the name suggests - for ISPs only and cannot possibly capture every single mail server. For company domains, universities and so on, please see the Autoconfig spec how to host the configuration yourself on your domain, and complying mail apps can find it automatically.

## Autoconfig

This ISPDB is part of a larger Autoconfig mechanism, which is described by Internet Draft [Autoconfig](https://www.ietf.org/archive/id/draft-ietf-mailmaint-autoconfig-00.html). Please see that document for a description of the exact file format, how to interpret it, and which other mechanisms you can use for smaller domains.

More information can be found on the [old Autoconfig website](https://www.bucksch.org/1/projects/autoconfiguration/).

## Information

All the server configuration needed to connect to the account should be included here. This includes:
* Which protocols are available
* Hostnames, ports, SSL config, or URL
* Authentication method (password, SCRAM, OAuth2, passkey etc.)
* Which username form (foo or foo@example.com or EXAMPLE\foo or similar)
* OAuth2 issuer, endpoints, scopes, client ID etc.
* Which other complimentary services are offered and available for this account, e.g. calendar, contacts, file sharing via WebDAV etc.

## Origin

This database was created by [Ben Bucksch](https://www.bucksch.org) and his company. Ben Bucksch came up with the idea of the ISPDB, that is to automatically look up authorative provider info during mail config setup, created the first ISPDB with its entries and data, created the Autoconfig standard, and created the first mail app implementation of it. This database is now a new re-creation of the database, from scratch, with the most current data from 2025, gathered directly from the ISPs, and validated with tests. Thanks to [Jeremy Chang](https://github.com/jermy-c) for the help getting this done.

