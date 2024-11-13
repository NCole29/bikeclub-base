# Bike Club - Base Repository 

## Overview

The base repository is the first step in setting up the Bike Club website **AFTER** you have installed Drupal and CiviCRM.

To install a new Drupal site with CiviCRM in your local development environment, use the scripts located in **[bikeclub/bikeclub-scripts](https://github.com/NCole29/bikeclub-scripts)**.

After installing Drupal you are ready to apply this recipe.

## How to Apply this Recipe

Use a terminal window in your local development environment (e.g., the terminal window in VS Code) to issue each of the following commands. 

	ddev composer config repo.bikeclub-base git "https://github.com/NCole29/bikeclub-base"
	ddev composer require bikeclub/bikeclub-base:1.0.2
	ddev exec php core/scripts/drupal recipe recipes/contrib/bikeclub-base
	
Description:	
1. "ddev composer config" adds the bikeclub repository to your composer.json file.
2. "ddev composer require" downloads the bikeclub repository to the web/recipes/contrib folder. 
3. "ddev exec php" executes the drupal script to apply the bikeclub-base recipe to the site.
	
Note: Step 2 will download all bikeclub recipes because they are all listed in the  bikeclub-base/composer.json file. We recommend that you *apply* recipes individually.

## Included in the Base Recipe

 - Core recipes: "core_recommended" recipes for maintenance, and performance; basic_block_type; image_ and document_media_type, and standard_responsive_images.
 - Additional core modules including menu, taxonomy, and views.
 - Contributed modules to enhance the administrative menu (admin_toolbar), allow login with email addresses (mail_login), manage menus (menu_admin_per_menu, menu_blocks), and create webforms (webform plus webform submodules).

## Sub-Repositories / Recipes downloaded with this base recipe

1. **[bikeclub/bikeclub-civicrm](https://github.com/NCole29/bikeclub-civicrm)**
	- Installs Drupal modules to integrate CiviCRM with Drupal:
	  civicrm_entity, civicrm_group_roles, civicrm_member_roles, civicrmtheme, webform_civicrm
	
2. **[bikeclub/bikeclub-media](https://github.com/NCole29/bikeclub-media)**
	- Installs media types and configuration for files and images. Four image types are configured with specific aspect ratios: banners (20:7), gallery images (3:2), images to insert in the editor (16:9 and 4:3).
	- Installs file and image taxonomies to categorize files.
	
