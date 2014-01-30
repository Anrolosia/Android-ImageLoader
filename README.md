Android-ImageLoader
===================

Android-ImageLoader is an Open Source Android library that allows developers to easily get and display
distant pictures using cache

Android-ImageLoader is currently used in some awesome Android apps. Here's a list of some of them:
* [Ma Filmotheque][1]

If you are using Android-ImageLoader in your app and would like to be listed here, contact me, I'd be happy to
list your app here!

Setup
-----
* Import Android-ImageLoader as an Android library project.
* Add dependency in your settings.gradle file
```java
include ':Libraries:Android-ImageLoader:imageloader'
```
* Add dependency in your build.gradle file
```java
dependencies {
  [...]
  compile project(':Libraries:Android-ImageLoader:imageloader')
}
```

How to use it
-------------
In order to use Android-ImageLoader into your own project, you have to create a Android-ImageLoader object with
some parameters:
* Context context: The application context (mandatory)
* String pathExtension: If you want to customize cache folder path, null as default value (optional)
* String cacheFolderName: Cache folder name (mandatory)
* int loadingPictureResource: Resource ID to display while loading remote picture, -1 as default value (optional)
* int noPictureResource: Resource ID to display if remote picture's loading failed, -1 as default value (optional)
* ImageView.ScaleType loadingScaleType: Scale type of the loading picture, null as default value (optional)

Then you have to call displayImage method with some parameters :
* String url: Remote picture url (mandatory)
* ImageView imageView: ImageView to display remote picture (mandatory)
* int requiredSize: Size of the compressed displayed picture, -1 for no compression (optional)
* ImageView.ScaleType scaleType: Scale type of the displayed picture (mandatory)

Developed By
------------
* Benjamin Moreau

License
-------

    Copyright 2014 Benjamin Moreau
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

[1]: https://play.google.com/store/apps/details?id=fr.moreaubenjamin.filmotheque
