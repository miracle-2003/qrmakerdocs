# Set up your site

## Change Favicon

1. Login as admin
2. Go to Settings-&gt;images
3. Upload your favicon



## Change the project logo and default images

Go to your project and login as admin.   
In the settings page, you will be able to change the project logo and the default images for the menu items and the cover image in the restaurant menu. 

## Change email send by the system

If you go to this folder **app/Notifications**

There are list of PHP files that represent the content of the email And inside them, there is function called **toMail**

You can modify the strings there.

If you want to change the layout, ex, include some CSS for the email you can edit the blade file here **resources/views/vendor/notifications/email.blade.php**

## **Change the content of the front page**

The landing page code is located in **resources/views/qrsaas.** If you want to do structural changes you can edit those files there. In our updates, we try not to change these files as much as possible. But for just in case, make a backup of them when you have done your changes.

If you want to change the css, the best way to do that will be throught the option to add custom CSS inside Admin-&gt;Setting-&gt;CSS and JS. There you can define your own CSS and JS, so if we have an update on our CSS or JS doesn't discard your changes. 

To modify the images, you can do that from Admin-&gt;Settings-&gt;Images.

To change the text, you can do that via the inline editing tool on the front page if you login as admin.

## Add more download print templates / change existing

At the moment, manually upload your zip of template directly in the "**public**" folder or create a new folder in there. You can also upload the zip in some File Storage like Google Drive, One Drive etc..   
Then, get the link to the zip file, and in your .ENV editor add or edit variable **linkToTemplates** that will link to the zip. 

To change the images displayed there, upload the images to the public folder or in some image share tool like Imgur.  Get the links and enter them as .ENV variable templates, comma-separated. 

ex

```text
linkToTemplates="/impactfront/img/templates.zip"
templates="/impactfront/img/menu_template_1.jpg,/impactfront/img/menu_template_2.jpg"
```

## How to disable landing page

In your .env editor add new variable DISABLE\_LANDING and set it to true. Then only the dashboard will be shown. In this case, best will be the project to be installed in the subdomain. ex app.mydomain.com and on mydomain.com you to run your own site. It can be any Wordpress or HTML site. 

