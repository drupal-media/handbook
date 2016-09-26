# About Media entity

## Basic concepts

Media entity provides a 'base' entity for media. This is a very basic entity which can reference to all kinds of media-objects (local files, YouTube videos, Tweets, Instagram photos, ...). Media entity provides a relation between Drupal and the media resource. You can reference to/use this entity within any other Drupal entity.

This module attempts to provide the base storage component for the Drupal 8 media ecosystem.

Once installed, a new entity type will be available (type: "media").
Please note that the different "types" of entities (known as "bundles") will be provided by other contrib modules (see further on this manual).
The main media_entity module only defines the base API for other modules to build their own bundle-specific logic on the top of it.

Project page: (https://drupal.org/project/media_entity)

## Dependencies

- Drupal core (>= 8.1.0)
- [Entity](https://drupal.org/project/entity) (>= 8.x-1.0-alpha3)

## Maintainers
- Janez Urevc ([@slashrsm](https://github.com/slashrsm)) (https://drupal.org/u/slashrsm)
- Primož Hmeljak ([@primsi](https://github.com/primsi)) (https://drupal.org/u/primsi)
- Nguyễn Hải Nam (@jcisio) (https://drupal.org/u/jcisio)
- Boris Gordon (@boztek) (https://drupal.org/u/boztek)

## Get in touch
- (http://groups.drupal.org/media)
- IRC: #drupal-media @ Freenode
