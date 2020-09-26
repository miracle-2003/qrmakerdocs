# Set up your site

## Change Favicon

Since this is PWA app, the best way to change the favicon together with the icon used in the PWA app is to use the Real Favicon generator \( [https://realfavicongenerator.net/](https://realfavicongenerator.net/) \)

Then upload your icon with at least 260x260 size.  PNG or JPG. 

Then go over the listing, and make sure you icon looks good. You ca also enter app name there. 

![](../.gitbook/assets/favicon%20%281%29.png)

Next, download the Favicon package. This zip contains all the needed favicons for both the site and the PWA. 

You can upload the zip, and extract in the **public** folder. Or Export locally and upload the files in the public folder.

## Change project logo and default images

Go to your project and login as admin.   
In the settings page, you will be able to change the project logo and the default images for the menu items and the cover image in the restaurant menu. 

## Change email send by the system

If you go to this folder **app/Notifications**

There are list of PHP files that represent the content of the email And inside them, there is function called **toMail**

You can modify the strings there.

If you want to change the layout, ex, include some CSS for the email you can edit the blade file here **resources/views/vendor/notifications/email.blade.php**

## **Change the content of the front page**

The landing page is single page. And also all the content is placed in single file.   
To edit your landing page open **resources/views/qrsaas/plan.blade.php**

This is a blade file, combination of laravel directives, and standard php and html.

## Add more download print templates / change existing

At the moment, manually upload your zip of template directly in the "**public**" folder or create new folder in there. You can also upload the zip in some File Storage like Google Drive, One Drive etc..   
Then, get the link to the zip file, and in your .ENV editor add or edit variable  **linkToTemplates** that will link to the zip. 

To change the images displayed there, upload the images to the public folder or in some image share tool like Imgur.  Get the links and enter them as .ENV variable templates, comma separated. 

ex

```text
linkToTemplates="/impactfront/img/templates.zip"
templates="/impactfront/img/menu_template_1.jpg,/impactfront/img/menu_template_2.jpg"
```

## How to disable landing page

In your .env editor add new variable DISABLE\_LANDING and set it to true. Then only the dashboard will be shown. In this case, best will be the project to be installed in subdomain. ex app.mydomain.com and on mydomain.com you to run your own site. It can be any Wordpress or HTML site. 

