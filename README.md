# Bike Club - Base Repository 
Link to github: [bikeclub/bikeclub-base](https://github.com/NCole29/bikeclub-base)

## Overview

Begin the Bike Club Drupal install here. This recipe installs part of the Drupal core Standard Profile plus key contributed modules to support administrative functions for the site.

After applying this recipe, continue with sub-repositories in the order listed.

## Included in this Base Recipe

 - Core recipes: "core_recommended" recipes for themes, maintenance, and performance; basic_block_type; image_ and document_media_type, and standard_responsive_images.
 - Additional core modules including menu, toolbar, taxonomy, and views.
 - Contributed modules to enhance the administrative menu (admin_toolbar), allow login with email addresses (mail_login), manage menus (menu_admin_per_menu, menu_blocks), and create webforms (webform plus webform submodules).

## Sub-Repositories / recipes installed by this base recipe:

1. **[bikeclub/bikeclub-media](https://github.com/NCole29/bikeclub-media)**
	- Installs media types and configuration for files and images. Four image types are configured with specific aspect ratios: banners (20:7), gallery images (3:2), images to insert in the editor (16:9 and 4:3).
	- Installs file and image taxonomies to categorize files.
		  
2. **[bikeclub/bikeclub-user-roles](https://github.com/NCole29/bikeclub-user-roles)**
	- Installs roles and permissions for: member, ride leader, membership coordinator, rides coordinator, and site_administrator.

3. **[bikeclub/bikeclub-civicrm](https://github.com/NCole29/bikeclub-civicrm)**
	- Installs CiviCRM plus related modules and configurations.
	- Related modules: civicrm_entity, civicrm_group_roles, civicrm_member_roles, civicrmtheme, webform_civicrm.