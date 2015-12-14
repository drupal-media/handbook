# Instagram

Implements media entity resource provider for Instagram photos and videos.

Project page: (https://drupal.org/project/media_entity_instagram)

## Requirements

1. [Media Entity](https://www.drupal.org/project/media_entity)

## Installation

1. Download [Media Entity](https://www.drupal.org/project/media_entity) from Drupal.org.
2. Download [Media Entity Instagram](https://drupal.org/project/media_entity_instagram) from Drupal.org.
3. Install both Media Entity Instagram and Media Entity in the [usual way](https://www.drupal.org/documentation/install/modules-themes/modules-8).

## Overview

Instagram field formatter can be used with three different types of fields:
* Text plain fields `string_long`, `string_short`
* Link fields
* Entity reference that references appropriate media bundles

In the **Usage** section configuration of media bundles and supported field types will be described in detail.

## Usage

1. Create a Media bundle
  * On `admin/structure` choose **Media bundles**
    ![Step 1](images/instagram/step_1.png)
  * Click on **+ Add media bundle**
    ![Step 2](images/instagram/step_2.png)
  * Fill *Label*, *Description* and *Type provider fields* for your media bundle and click **Save media bundle**
    ![Step 3](images/instagram/step_3.png)
2. Create an Instagram link field on a Media bundle
 * On media bundles overview page choose **Manage fields** on created **Instagram** bundle.
   ![Step 4](images/instagram/step_4.png)
 * Click on **+ Add field**. For a storage type choose **Link**, fill a *Label* field and click **Save and continue**.
   ![Step 5](images/instagram/step_5.png)

2. Create a Media entity
  * On `admin/content/media` click on **+ Add media**
    ![Step 6](images/instagram/step_6.png)
  * Fill *Media name*, *Instagram link* fields similarly as it is displayed below and click **Save**.
    ![Step 7](images/instagram/step_7.png)
  * The created Instagram media entity is saved.
  
    ![Step 8](images/instagram/step_8.png)
3. Add an entity (media) reference field on a content type
  * On desired content type (i.e. Article), on `admin/structure/types`, click on **Manage fields**
    ![Step 9](images/instagram/step_9.png)
  * Click on **+ Add field**
    ![Step 10](images/instagram/step_10.png)
  * From **References** menu choose **Other**, fill the *Label* and click **Save and continue**
    ![Step 11](images/instagram/step_11.png)
  * Choose **Media** for **Type of item to reference** and click **Save field settings**
    ![Step 12](images/instagram/step_12.png)  
  * Select **Instagram** bundle in **Reference type section** and click **Save settings**
    ![Step 13](images/instagram/step_13.png)      
4. Add a Text plain (long) field on a content type
  * Repeat the first two steps from the section below. Select **Text (plain, long)** from **Add a new field** menu, fill the *Label* and click **Save and continue**
  ![Step 14](images/instagram/step_14.png)
5. Add a Link field on a content type
  * Go to **Add a new field** page by following the steps from **Step 3**. Select **Link** from **Add a new field** menu, fill the *Label* and click **Save and continue**
  ![Step 15](images/instagram/step_15.png)  
5. Open Manage display of your content type (in our case *Article*), on `admin/structure/types/manage/article/display`
  * Select **Instagram embed** for the three freshly created fields (*Text plain*, *Link*, *Entity media reference*) and then **Save**
  ![Step 16](images/instagram/step_16.png)
6. Create a new article with embedded Instagram posts
  * For an **Instagram reference** field choose a created entity Instagram entity. **Text** and **Link** fields fill with URLs to Instagram posts.
  ![Step 17](images/instagram/step_17.png)  
  * The Instagram posts are displayed on the saved article page.
