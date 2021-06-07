---
title: Token Manager
---

The token is a hexadecimal access code that allows the upload of imagery to the OAM database.
Administrators can create and manage tokens using the [admin interface](https://admin.openaerialmap.org).

![Screenshot](/content/uploader/token-create.png)


Since tokens are not tied to a specific user, a description allows the admin to keep track of the purpose of each one.

Tokens can have an expiracy date, a feature that is useful if the token is being generated, for example, for a mapping event. They can also be temporarily blocked and/or revoked when needed.


![Screenshot](/content/uploader/token-manager.png)


### Source code and development
The `oam-uploader-admin` is completely open source and the [code and instructions](https://github.com/hotosm/oam-uploader-admin) are available on github under the **BSD 3-Clause license**.
