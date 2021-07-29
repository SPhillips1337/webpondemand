# webpondemand
PHP Script to convert any image to webp on demand.

* Original version of the function is from JC Labs https://www.jclabs.co.uk/generate-webp-images-in-php-using-and-gd-or-imagick/ I updated it with a fix so that the webp files created using the built in PHP GD Library are generated correctly now, so that the script works and the resulting files can be viewed and are not broken.

* I added some code to make this work with a .htaccess file using mod rewrite so that a variable called source gets passed to the script, and also updated the script to use this variable, if a webp image is found or generated then it passed through with mime type headers to be loaded by the browser.

* I updated so all converted images are placed into a folder called webp in the same folder as the script

Installation
============
Drop the script and htaccess at the top level of a website where you want to use them (Or merge the htaccess with your current one) to then convert and use webp images on the fly.

Example url based usage;

http://www.stephenphillips.co.uk/webpondemand/webpondemand.php?source=test.jpg

Included in these files are a test.jpg and a test.png in the root folder.

Requirements
============
You will need PHP 5.5 or higher and GD library enabled or Image Magik.
