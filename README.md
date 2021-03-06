# FileMaker WebDirect Custom Homepage #

This repository has been provided by [Harlow Technologies Inc.](http://www.harlowtech.com) as a service to the FileMaker community in making FileMaker WebDirect logins for our customers easier.

Below are the instructions for how to install and configure the HTML pages for custom FileMaker WebDirect login and logoff pages.

## Installation ##

* Install Instructions
* Web Directory Root Folder
* How to Download these Files

### Install Instructions ###

1. After downloading the files, open the index.html and logoff.html in a text editor.
2. On both files, make the following adjustments:
    1. If you are using https, update the url protocol to https from http on both the URL and URL parameter “homeurl”.
    2. Update the web host (example: fms.example.com) to the host name or IP you wish to use for the FileMaker Server.
    3. Update the web host (example: web.example.com) to the host name or IP you wish to use for URL parameter "homeurl"
    4. Update the folder name to the folder name you wish to use on the web server in the URL parameter "homeurl" for the logoff page.
    5. Update the database name after the # sign in the URL parameter "homeurl"
3. Place the folder on the web server root folder and provide the user with the URL to the index.html file.
4. Give the user your adjusted URL to start using FileMaker WebDirect with a custom home page Example: http://web.example.com/mysolution/index.html

### Web Directory Root Folder ###

The typical web server root folders for FileMaker Server can be found at:

__For IIS (Windows) through HTTP or HTTPS__

* [drive]:\Program Files\FileMaker\FileMaker Server\HTTPServer\conf
* Where [drive] is the drive on which the Web Publishing Engine component of your FileMaker Server deployment resides.

__For Apache (OS X) through HTTP__

* /Library/FileMaker Server/HTTPServer/htdocs

__For Apache (OS X) through HTTPS__

* /Library/FileMaker Server/HTTPServer/htdocs/httpsRoot

### How to Download these Files ###

Want to download and try these files out with your solution. Look for the "Download ZIP" link to the on the right hand side on [GitHub](https://github.com/bharlow/fm-webdirect-custom) page.

## Tips and Hints ##

When you update the web host or folder name the index.html needs to have it updated in two locations while the logoff.html only has one location.

The URL Host Name or IP for the FileMaker Server can be different than the homeurl URL Host Name or IP. You must be sure to link the pages up appropriately.

The full web direct guide can be found at [FileMaker WebDirect PDF](https://fmhelp.filemaker.com/docs/13/en/fm13_webdirect_guide.pdf). Page 27 in the guide has official instructions on using the WebDirect custom homepage.

## Change Notes ##

* Version 0: 05/14/2014 - Initial Creation and deployment
* Version 1: 07/24/2014 - Addition of JavaScript Redirect to index.html

## Copyright ##

Copyright 2014 Harlow Technologies Inc.

* Released under the MIT license
* https://github.com/bharlow/fm-webdirect-custom/blob/master/LICENSE.txt

FileMaker is a trademark of FileMaker, Inc., registered in the U.S.and other countries. FileMaker WebDirect is a trademark of FileMaker, Inc.