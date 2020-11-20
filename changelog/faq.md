---
description: Frequently Asked Questions (FAQs)
---

# FAQ

## Registration is not working.

This is one of the most common problem. It happens because SMTP is not correctly set up, or not setup at all. To learn how to set it up, follow this guide

{% page-ref page="../define-basics/obtain-smtp.md" %}



## How restaurants owner register?

At the fronted part of the script you will find the form for  **Registration.** . The interested restaurants will fill the form, and Restaurant / owner account will be automatically created. Email will be send to them.

The restaurant owner will need to login with the email and password \(generated password can change if he wants in profile page\). After that the owner can start filling the items / categories for his restaurant.

Initially they are assigned to free plan. 



## What languages the site works in?

The site operates in 1 language that can be defined from the .env variable. We have the site translated in

* [x] English
* [x] French
* [x] German
* [x] Spanish
* [x] Italian
* [x] Russian
* [x] Portuguese 

Easy to translate to any language. All strings are in 1 file.



## What technology is used?

### WEB \( Storefront and Dashboard \)

* Laravel - PHP Framework
* MySQL Database
* Bootstrap - Based on Argon Design from Creative Tim
* React JS
* Mobile ready - Both storefront and dashboard



## How to delete the demo data?

To delete the demo data go to your site Adminer. \(Adminer is php script to manage your database\).  
The Adminer is located on **yourdomain.com/adminer**

There, login with your database username and password.  
Click on the SQL command icon \( [Image](https://i.imgur.com/GXetB8K.png) \)

In the text area enter the following sql command. After executing [THIS](https://gist.github.com/dimovdaniel/ebbaa2bb379e92bfc1e223b306ca1531) commands, only your admin user will remain in the database.

## What are the benefits for different stakeholders. 

### Benefits for project owner

1. Start a subscription business in less than 10 min
2. Robust solution with no additional monthly charges or any extra service need.
3. No time need to run this business. It is completely automated and scalable. 
4. Take advantage of this pandemic, and turn it into your favor. 

### Benefits for restaurants

1. Offer they guests clean and modern solution to see their menu. Regular print menus are touched with up to 100 hands per day 🦠. 
2. Paper menu is getting ruined quickly. So they need to reprint. With QR Menu the qr card or sticker is protected and can last lot longer. 
3. For any new dishes, using print menu, they need to reprint their menu, or introduce new sheet of paper in their menu. With QR Menu, they just go to the website and update the menu. 
4. ECO friendly. I big restaurant menu = 1 tree 🌲. Yes, for real.
5. Restaurants can share their menu online.  Based on [a research conducted by OpenTable](https://go.opentable.com/rs/531-AOS-877/images/OpenTableTechnologyAndDiningOut2015l.pdf), 86% of customers regularly check out menus online before they dine out. 

### Benefits for clients

1. Super clean solution. Using their phone, they just scan the QR, and they see the menu. No mobile app required. 
2. They will not touch a thing that is being touched with 100 different hands in one day 🦠.
3. No need to wait for waiter just to bring the menu. 
4. Sometimes, on bigger tables, guests need to wait for other to read the menu, and then pass to them. No more, using their phones everyone can have the menu instantly. 
5. According to a study, 20% of the print menu prices aren't up to date. With QR menu, they will always see up today prices and menu items. 
6. They will be able to quickly see the correct item price. They are able to select different item variants and variant's extras.

## Common problems

### Error on update

**Problem**: After an update, some users experience error 503 \| Service not found.

**Cause**: This mostly happens because your PHP setup doesn't have the ZIP extension enabled. 

**Solution**: 

You will need to enable the ZIP extension 

This is the best and simplest guide we could find on how to enable the ZIP extension in cPanel

{% embed url="https://bobcares.com/blog/enable-php-zip-extension-cpanel/" %}

Also, please talk with your hosting provider on how to enable the zip extension for you.

## Error 500

**Problem**  
You get a white screen with Error 500 on it 

**Reason**  
This is a general error, meaning something wrong happened in the system. And it can be from different causes. it can be a bug or misconfiguration. 

**Solution**  
First, we need to see why this error happens,   
Enable debug mode, so you can see what is behind the 500 error. To do that

1. Login as admin
2. Go In **Setting**
3. Select **Settup** tab
4. Select **APP\_DEBUG**

Then try to reproduce the problem. Now, you will see a lot more information about the problem. If you do understand the message, you get, you may fix the problem on your own. Some common ones are SMTP are Stripe Misconfiguration. For these ones you may try to fix on your own, by going in settings to check if what you have entered is correct. 

For some other reported errors, don't hesitate to contact us with a screenshot of the problem \( including the address bar link \) here [https://help.mobidonia.com/\#qrsaas](https://help.mobidonia.com/#qrsaas)

## SQL Error - Table not found

**Error**   
After installation, when you open your site, you see an error screen with a report similar to this.

```text
local.ERROR: SQLSTATE[42S22]: Column not found: 1054 Unknown column 'plan.plan_id' 
```

**Reason**  
The most common problem for this is because you have entered the wrong credentials/user/pass for the Database and the setup of the database was incomplete. 

**Solution**

1. Open the file **.env** and make sure you have entered the correct  DB data
2. Remove file storage/installed
3. Try to install again by visiting yourdomain.com/install

If that doesn't help, please create a ticket, and if you can share cPanel / Admin details with us so we can look into the problem. 



## Error on uploading an image 

**Error**

"PHP Fileinfo extension must be installed

**Reason**  
 "PHP Fileinfo extension must be installed/enabled to use Intervention Image."

The project needs the [fileinfo](https://i.stack.imgur.com/vhN3E.png) extension. 

**Solution**

As you can see on the [image](https://i.stack.imgur.com/vhN3E.png), it can be enabled from PHP Selector. But if there is no  PHP Selector you should have access to **WHM**.

**IN WHM**

Initially, we login to WHM and navigate as follows,

Software &gt;&gt; EasyApache 4 &gt;&gt; Customize &gt;&gt; PHP extensions.

Here we search for **fileinfo** and enable phpx.x-php-fileinfo for all versions. Finally, we click on Review and Provision.

This enables the file extension for all the PHP websites in the server.

Let me know about this.











