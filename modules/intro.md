#D8 Media Modules

There is a substantial amount of media functionality available in Drupal 8 today. This section of the guide provides a brief summary of the functionality delivery by each module and its current status.

## D8 Core Functionality

In Drupal 8 core, As in D7 core, there is out of the box support for files, images and basic media functionality. That said rich media experiences in Drupal are generally built using the contributed modules listed below.


## D8 Contrib  Modules 

As discussed in the introduction to this guide, the Drupal 8 Media ecosystem includes several independent but interoperable/pluggable Media modules.

The modules are intended to be uses together as needed in order to provide as basic or advance a media solution as is needed for a particular Drupal project.


###D8 Media Storage Modules

* [**File Entity:**](modules/file_entity/intro.md) provides interfaces for storing and managing files, which extends core file entity e.g., allowing for file fields, types, display modes, etc. ([d.o](https://github.com/drupal-media/file_entity))
 * *Latest Status:* TBA


* [**Media Entity:**](modules/media_entity/intro.md) an alternate approach to media storage in Drupal, which doesn't directly extend core file entity ([d.o](https://www.drupal.org/project/media_entity))
 * *Latest Status:* TBA


* [**Flysystem:**](modules/flysystem/intro.md) provides a bridge to use Flysystem as Drupal stream wrappers ([d.o](https://www.drupal.org/project/flysystem))
 * *Latest Status:* TBA


###D8 Media U/I Modules

* [**Crop API:**](modules/crop/intro.md) an API for image cropping that's intended to be used with a related API module such as [Image Widget Crop]( https://www.drupal.org/sandbox/woprrr/2571403) ([d.o](https://www.drupal.org/project/crop))
 * *Latest Status:* TBA


* [**DropzoneJS:**](modules/dropzonejs/intro.md) provides drag ’n’ drop file uploads with image previews ([d.o](https://www.drupal.org/project/dropzonejs))
 * *Latest Status:* TBA


* [**Embed API:**](modules/embed/intro.md) a framework module to embed things using the Drupal 8 WYSIWYG editor ([d.o](https://www.drupal.org/project/dropzonejs))
 * *Latest Status:* TBA


* [**Entity Browser:**](modules/entity_browser/intro.md) provide a generic browser that can be used for selecting file/media entities.
 * *Latest Status:* TBA


* [**Entity Embed:**](modules/entity_embed/intro.md) allows any entity to be embedded within a text area using a WYSIWYG editor.
 * *Latest Status:* TBA


* [**File Entity Browser:**](modules/file_browser/intro.md) provides a nice content creator/editor experience for uploading files (implementing [Dropzonejs](https://www.drupal.org/project/dropzonejs)) and browsing/selecting files (implementing [Entity Browser](modules/entity_browser/intro.md).
 * *Latest Status:* TBA


* [**Image Widget Crop:**](modules/image_widget_crop/intro.md) provides an interface for using the features of the [Crop API](https://www.drupal.org/project/crop) ([d.o](https://www.drupal.org/sandbox/woprrr/2571403))
 * *Latest Status:* TBA


* [**URL Embed:**](modules/url_embed/intro.md) allows embedding of URLs using the Drupal 8 WYSIWYG or link fields ([d.o](https://www.drupal.org/project/url_embed))
 * *Latest Status:* TBA


###D8 Media Display Modules

* [**Fallback Formatter:**](modules/fallback_formatter/intro.md) a field formatter that attempt multiple formatters for displaying file and applies the first one that returns output ([d.o](https://www.drupal.org/project/fallback_formatter))
 * *Latest Status:* TBA

 
* [**Field Formatter:**](modules/field_formatter/intro.md) a field formatter that attempt multiple formatters for displaying file and applies the first one that returns output ([d.o](https://www.drupal.org/project/field_formatter))
 * *Latest Status:* TBA


###D8 Media Feature Modules

* [**Media Pinkeye:**](modules/media_pinkeye/intro.md) one of the "full-featured" media solutions for Drupal 8. It's goal is to provide basic media features and experience (WordPress parity) ([d.o](https://www.drupal.org/project/media_pinkeye))
 * *Latest Status:* TBA
 
 
 
 