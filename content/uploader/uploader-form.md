---
title: Uploader Form
bookShowToC: true
type: pages
---

The upload form is the way for users to contribute to the OAM imagery database.
Besides uploading the imagery itself, contributors need to provide metadata for imagery datasets.
There are two types of fields for filling in the metadata: fields for input values (Title, Sensor, Provider, Tags, Contact info) and fields with choices (Platform, Date start, Date end, Contact, License).


![Screenshot](/content/uploader/form.png)


Also, there is an opportunity to upload several imagery datasets by clicking on the "New dataset" button.

![Screenshot](/content/uploader/new-dataset.png)


## Contributing

In order to upload imagery to OAM, you have two options for storing your files. One option is to have your files stored in a publicly accessible location, which means they cannot be stored only on your computer but need to be stored in a location that allows downloads. Services like [Dropbox](https://www.dropbox.com) and [Google Drive](https://drive.google.com) provide easy-to-use file storage with methods for public sharing.
Alternatively, you can also upload files directly from your local device. This means you can select and upload files that are stored on your computer without the need for them to be in a publicly accessible location.

### via Dropbox

If you have your imagery stored in Dropbox, you can directly select the files you would like to upload from the Dropbox file integration. 

Select Dropbox as your Imagery Location, and Dropbox will open a dialog box to authorize and allow you to select individual files to share. Multiple files can be selected. 

Please be aware that Dropbox automatically turns on file sharing for each file selected temporarily.

### via Google Drive

You can connect your Google Drive folder and individually select files to be uploaded. In order for OAM to download the file from Google Drive, each file must have sharing settings that allow the file to be publicly viewable. Follow these steps if the file does not have sharing turned on: 

1. Navigate to your Google Drive folder
2. Right click on the file(s) you want to share and select "Share"
3. Within the "Share with others" window, select "Advanced"
4. The window will change to the "Sharing settings", click "Change" for "Who has access"
5. Select "On - Public on the web" or "On - Anyone with the link" to enable public sharing
6. Ensure "Access:Anyone (no sign-in required)" is set to "Can View"

Read more on the [Google Drive support forum](https://support.google.com/drive/answer/2494822?hl=en&ref_topic=7000947).

### via public URL

If you have files stored in another location, copy and paste the full URL (including "http") into the Upload form box. These file locations need to be publicly accessible, meaning that anyone with the link can download from that location.

### via Local Device

Users can also upload imagery from their local devices. The system suggests files in `TIFF` and `TIF` formats by default. To initiate the upload, select the desired files from your device and then submit the form. Once submitted, the uploading process will begin.


## Source code and development
The `oam-uploader` is completely open source and the [code and instructions](https://github.com/hotosm/oam-uploader) are available on github under the **BSD 3-Clause license**.
