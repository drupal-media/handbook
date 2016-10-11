#D8 Media Modules

There is a substantial amount of media functionality available in Drupal 8 today. This section of the guide provides a brief summary of the functionality delivery by each module and its current status.

## D8 Core Functionality

In Drupal 8 core, As in D7 core, there is out of the box support for files, images and basic media functionality. That said, rich media experiences in Drupal are generally built using the contributed modules listed below.


## D8 Contrib  Modules 

As discussed in the introduction to this guide, the Drupal 8 Media ecosystem includes several independent but interoperable/pluggable Media modules.

The modules are intended to be used together as needed in order to provide as basic or advanced a media solution as is needed for a particular Drupal project.


###D8 Media Storage Modules

* [**File Entity:**](file_entity/intro.md) provides interfaces for storing and managing files, which extends core file entity e.g., allowing for file fields, types, display modes, etc. ([d.o](https://www.drupal.org/project/file_entity))
 * *Latest Status:* Beta


* [**Media Entity:**](media_entity/intro.md) an alternate approach to media storage in Drupal, which doesn't directly extend core file entity, and creates a new entity type to be served as a base for other modules (providers) to build upon and define their own media types. ([d.o](https://www.drupal.org/project/media_entity))
 * *Latest Status:* Stable (general availability) release


* [**Flysystem:**](flysystem/intro.md) provides a bridge to use Flysystem as Drupal stream wrappers ([d.o](https://www.drupal.org/project/flysystem))
 * *Latest Status:* Alpha


###D8 Media UI Modules

* **Content Browser:** provides a nice content creator/editor experience for browsing and selecting existing content (nodes). It is built upon the [Entity Browser](modules/entity_browser/intro.md) module, improving the UI and providing a pre-configured browser out-of-the-box. ([d.o](https://www.drupal.org/project/content_browser))
 * *Latest Status:* Alpha


* [**Crop API:**](crop/intro.md) an API for image cropping that is intended to be used with a related API module such as [Image Widget Crop]( https://www.drupal.org/project/image_widget_crop) ([d.o](https://www.drupal.org/project/crop))
 * *Latest Status:* Stable (general availability) release


* [**DropzoneJS:**](dropzonejs/intro.md) provides "drag & drop" file uploads with image previews ([d.o](https://www.drupal.org/project/dropzonejs))
 * *Latest Status:* Alpha


* [**Embed API:**](embed/intro.md) a framework module to embed things using the Drupal 8 WYSIWYG editor ([d.o](https://www.drupal.org/project/embed))
 * *Latest Status:* RC (release candidate)


* [**Entity Browser:**](entity_browser/intro.md) enables the creation of user-friendly browsers that can be used for selecting entities (file, image, media entities, etc). ([d.o](https://www.drupal.org/project/entity_browser))
 * *Latest Status:* Alpha


* [**Entity Embed:**](entity_embed/intro.md) allows any entity to be embedded within a text area using a WYSIWYG editor. ([d.o](https://www.drupal.org/project/entity_embed))
 * *Latest Status:* Beta


* [**File Entity Browser:**](file_browser/intro.md) provides a nice content creator/editor experience for uploading files (implementing [Dropzonejs](https://www.drupal.org/project/dropzonejs)) and browsing/selecting files (implementing [Entity Browser](modules/entity_browser/intro.md)). ([d.o](https://www.drupal.org/project/file_browser))
 * *Latest Status:* Alpha


* [**Image Widget Crop:**](image_widget_crop/intro.md) provides an interface for using the features of the [Crop API](https://www.drupal.org/project/crop) ([d.o](https://www.drupal.org/project/image_widget_crop))
 * *Latest Status:* Stable (general availability) release


* **Media Entity Browser:** provides a nice content creator/editor experience for browsing and selecting existing media entities. It is built upon the [Entity Browser](modules/entity_browser/intro.md) module, improving the UI and providing a pre-configured browser out-of-the-box. ([d.o](https://www.drupal.org/project/media_entity_browser))
 * *Latest Status:* TBA


* [**URL Embed:**](url_embed/intro.md) allows embedding of external URLs using the Drupal 8 WYSIWYG or link fields ([d.o](https://www.drupal.org/project/url_embed))
 * *Latest Status:* TBA


###D8 Media Display Modules

* [**Fallback Formatter:**](fallback_formatter/intro.md) a field formatter that attempts multiple formatters for displaying file and applies the first one that returns output ([d.o](https://www.drupal.org/project/fallback_formatter))
 * *Latest Status:* Stable (general availability) release

 
* [**Field Formatter:**](field_formatter/intro.md) provides a field formatter that can attempt multiple formatters and the first one that returns output wins. ([d.o](https://www.drupal.org/project/field_formatter))
 * *Latest Status:* Stable (general availability) release

* **Media Expire:** This module enables you to unpublish your media entites automatically by setting an expire field. ([d.o](https://www.drupal.org/project/media_expire))
 * *Latest Status:* Alpha

###D8 Media Feature Modules

* **[Media:](media/intro.md)** full featured media module for Drupal 8 which depends on other D8 modules to provide functionality. This module comes with lot of configuration files to provide most of the basic features. ([d.o](https://www.drupal.org/project/media))
 * *Latest Status:* TBA


* [**Media Pinkeye:**](media_pinkeye/intro.md) one of the "full-featured" media solutions for Drupal 8. It's goal is to provide basic media features and experience (WordPress parity) ([d.o](https://www.drupal.org/project/media_pinkeye))
 * *Latest Status:* TBA
 
 
 **NOTE**: The "Latest Status" information was last updated on **October, 11th, 2016**. You are encouraged to visit each module page to get potentially more updated information on its status.