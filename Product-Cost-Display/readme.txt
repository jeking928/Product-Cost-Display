-----------------------------------------------------------------

Zen Cart Mod: Product Cost Display
Released under the GPL license found in the root directory of this package.
Author: jandm-ent
Version: v1.0 (Original Release)
Zen Cart Compatibility: Only Tested for Zen Cart 1.5

-----------------------------------------------------------------

This Mod allows you to show your product cost (the cost to you from your vendor) on the product page in the admin area. This mod only displays in the admin area and does not display on the catalog. This mod is great for anyone who wishes to track product cost in Zen Cart with out having to keep an external list. You can also use this mod with Easy Populate 4.0 for easy cost updating by following our included instructions (No files of Easy Populate 4.0 are Changed).

-----------------------------------------------------------------

Included files:

New
Admin/includes/languages/english/extra_definitions/cost.php

Core Files
Admin/includes/modules/product/collect_info.php
Admin/includes/modules/copy_to_confirm.php
Admin/includes/modules/update_product.php

-----------------------------------------------------------------

Installation Instructions

Installing Product Cost Display is very simple.

1. Upload the included files to your admin folder (Be sure to change the name of the admin folder to the name of your admin folder).

BE SURE TO BACKUP YOUR ORIGINAL CORE FILES INCASE YOU WISH TO UNINSTALL!

2. In your admin area go to Admin>Tools>Install SQL Patches, Browse for and upload the included Product_Cost.sql file.

BE SURE TO BACKUP YOUR SQL DATABASE BEFORE DOING THIS STEP!

-----------------------------------------------------------------

Uninstall Instructions

If you decided you want to remove this mod, it's a case of reversing the actions above. 

1. Go to Admin>Tools>Install SQL Patches and copy, paste and run the following:

ALTER TABLE `products` DROP `products_cost`

2. Delete 
admin/includes/languages/english/extra_defintions/cost.php

3. Replace the following with the originals
admin/includes/modules/update_product.php 
admin/includes/modules/copy_to_confirm.php
admin/includes/modules/product/collect_info.php

-----------------------------------------------------------------

Easy Populate 4 Custom Field Instructions (Easy Populate 4.0.22 Beta)

1. Go to Admin>Configuration>Easy Populate 4

2. Edit User Defined Products Fields, Add products_cost

3. Update

Your export will now include a column called v_product_cost for easy updating

-----------------------------------------------------------------

Change Log:
July 7, 2012: V 1.0 New Mod 
