#Install

## Install Wordpress
https://de.wordpress.org/download/

Download and unzip the wordpress installation files. The files should be in the root folder of your server (or the directory you want to run the site from)!

## Install The Wordpress Plugins
Log into the admin area and install the following plugins
- Yoast SEO 
- Page Builder by SiteOrigin 
- SiteOrigin Widget Bundle
- Kadence Toolkit
- Polylang

## Install the parent theme
In the admin area, go to `Design` > `Themes` and install the `Virtue` theme.

## Copy the project files
In your file-system go to your wordpress directory `/wp-content/`.
- Copy the `virtue-child` directory to `themes/`
- Overwrite the `uploads` directory with the  the `uploads` directory of the project

## Activate the theme
In the admin area, go to `Design` > `Themes` and activate the `Virtue Child` theme.

## Setup the Database Content

### Save your user/password
Copy (backup) your password (column `user_pass`) from the `wp_users` table - you will need this later!! (it will be overwritten by the db import)
(for instance with phpMyAdmin)

### Import the DB
Import the sql file of the project to your database (for instance with phpMyAdmin)

### Adjust the DB Content
Install the "Database Search and Replace Script" from https://interconnectit.com/products/search-and-replace-for-wordpress-databases/

Open the Script in your browser.

Replace all occurences 
- `jaqueline.pelzer@chello.at` -> `YOUR_EMAIL`
- `http://localhost:2468/flipmouse` -> `URL_OF_YOUR_SITE`
- `/Applications/MAMP/htdocs/flipmouse/`-> `FULL_FILE_SYSTEM_PATH_TO_YOUR_SITE`
 
**Don't forget to remove the Script from your server, once everything is done!**

**---> NOW YOU CAN OPEN THE WEBSITE IN YOUR BROWSER!**

### Copy your user
Update the entry in the `wp_users` table with your login details.

**---> NOW YOU CAN LOG IN TO THE ADMIN AREA!**
