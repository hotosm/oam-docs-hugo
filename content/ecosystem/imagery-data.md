---
title: Data Structure
weight: 4
type: pages
---

## OpenAerialMap Data Layout and Structure

The imagery data that is uploaded to OAM is processed and stored into an AWS S3 Bucket with the following structure
```
<SceneID>/<UploadNum>/...
```
Each folder contains the following files:

| File        | Description |
| ----------- | ----------- |
| <ImageID>_meta.json	     | File metadata json file |
| <ImageID>.json	   | Image metadata json file      |
| <ImageID>.png	     | Thumbnail png                 |
| <ImageID>.tif      | Cloud Optimized GeoTIFF       |

Some older uploads also contain .msk and .vrt files as well. 

