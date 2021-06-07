---
title: OAM API
weight: 2
---

# OpenAerialMap API

OpenAerialMap API is an application programming interface (API) that serves metadata about available images and map layers. The API provides access to all imagery metadata information and endpoints to list images available, map layer services available, as well as simple analytics.

## Quick Start
The API is split into three available endpoints:

- a metadata endpoint `/meta`
- a tiled map service (TMS) listing endpoint `/tms`
- and an analytics endpoint `/analytics`

To get started, you can access the metadata endpoint here: [http://api.openaerialmap.org/meta](http://api.openaerialmap.org/meta). 

## Further documentation 
Check out the full [API documentation](http://hotosm.github.io/oam-api/) for methods to filter and limit results, get an individual image metadata, or add TMS endpoints to the listing.

## API status
Having the API up and running is crucial for the whole OAM Ecosystem. Its status is monitored and is available at [status.openaerialmap.org](http://status.openaerialmap.org).

## Source code and development
The `oam-api` is completely open source and the [code and instructions](https://github.com/hotosm/oam-api) are available on github under the **BSD 3-Clause license**.
