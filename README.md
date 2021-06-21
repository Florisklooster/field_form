# FieldForm

Perform location-bound measurements in the field

On Android:
https://play.google.com/store/apps/details?id=nl.artesia.field_form

On iOS:
link will follow when released

## Getting Started

Use FieldForm to conduct location-bound measurements in the field, store the values on your phone, and share the measurements with other people. To use FieldForm for a set of locations with multiple people simultaneously, the use of an FTP-server is recommended.

FieldForm is the successor to FieldLogger. It is build platform-independent in Flutter, so there are no differences anymore in functionality between the Android- and iOS-app. The new structure makes it easier to add functionality or fix bugs. FieldForm is now completely open source.

## For FieldLogger-users
There are some important changes between the files used or generated by FieldLogger and FieldForm. The file with location-data is a json file (instead of a csv in FieldLogger), to better incorporate the nested structure of the location-data. The measurement-data still consists of csv-files. The date-format however is changed to yyyy-mm-dd (instead of dd-mm-yyyy in FieldLogger), to minimise potential errors.

## For Developers
This repository holds the source code of FieldForm, with which the app can be built using Android Studio (and Xcode for iOS). Because of security concerns the signing keys are not added to this repository, so only specific developers are able to update the app in the Play Store and App Store. The source code can be used by any developer to test the app, or to release an app with another name.

Also, the Google Maps api-key is not contained in the repository. When building the app, the Google Maps api-key is taken from an environmental variable named 'maps_api_key', defined in the operating system that builds the app. To get a working Google Maps, a developer should therefore request an api-key at Google, and at this environmental variable.
