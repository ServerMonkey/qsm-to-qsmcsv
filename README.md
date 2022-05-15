# QSM to QSMCSV

Export QSM questions to CSV via command-line.

### Installation  
Install onto the same server as your Wordpress instance.  
Needs to run with the same user permissions, usually www-data.

### Configuration 
Create a config file (usually for the user www-data) in  
`~/.qsm-to/qsm-to-qsmcsv.cfg`  
You can use the file `/usr/local/share/qsm-to-qsmcsv/qsm-to-qsmcsv_default.cfg` as template.  
Fill in the following information:  
`USER` - Wordpress user with rights to export QSM to CSV  
`PASS` - Password for that Wordpress user  
`SITE` - Is the URL to that Wordpress webbserver, usually localhost.  
`PATH_RESULTS` - Path to the folder with the QSM export files. Usually something like:  
`/var/www/html/wordpress/wp-content/plugins/qsm-export-results/exports`  
`PATH_SAVE_TO` - Path to the folder where the quizzes will be stored.

### How to use  
Once configured just run it via a PHP script or from a shell:  
`qsm-to-qsmcsv`

Or run in debug mode:  
`qsm-to-qsmcsv debug`  

Example web templates can be found in the folder `web_templates`
