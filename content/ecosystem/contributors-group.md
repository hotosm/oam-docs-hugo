---
title: Contributors Group
bookShowToC: true
type: pages
---

# Contributor Components
 ![Screenshot](/content/ecosystem/ecosystem_oam_uploader.png)

Components that allow a contributor to add data to the system through an upload form. The data is added to the HOTOSM imagery bucket. Contributors with a large amount of imagery should consider [setting up their own imagery bucket](https://github.com/openimagerynetwork/oin-register) within the OIN network.

## OAM Uploader
A web form that a contributor can use to add datasets to OpenAerialMap.

- [Link to Github](https://github.com/hotosm/oam-uploader) 
- [Link to Documentation](/uploader/uploader-form/)

## OAM Uploader API
The OAM Uploader API is built using two sub-components. The worker processes uploaded imagery and pushes to an imagery bucket.

- [Link to Github](https://github.com/hotosm/oam-uploader-api)
- [Link to Documentation](/uploader/api-server)

### Worker subcomponent
Written in NodeJS

- Processes the jobs from the database. This is an asynchronous process that happens periodically.
- Generates final TIF images and metadata (following the Open Imagery Network specification) and uploads them to the HOTOSM OIN imagery bucket.
