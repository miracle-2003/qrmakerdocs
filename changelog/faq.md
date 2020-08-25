---
description: Frequently Asked Questions (FAQs)
---

# FAQ

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

## How to add new admin?

We have add the task - Admins to be able to add new admins from the interface. So it is not yet available

But here are the steps to do it now.

1. Register new client. 
2. Go in the database yourdomain.com/adminer and login
3. Get the ID of the user from **users** table
4. Go in **model\_has\_roles** table. There you should find that id  have **role\_id** 4. 
5. Change it to **role\_id** 1

Now he is admin.



## How to delete the demo data?

To delete the demo data go to your site Adminer. \(Adminer is php script to manage your database\).  
The Adminer is located on **yourdomain.com/adminer**

There, login with your database username and password.  
Click on the SQL command icon \( [Image](https://i.imgur.com/GXetB8K.png) \)

In the text area enter the following sql command. After executing [THIS](https://gist.github.com/dimovdaniel/ebbaa2bb379e92bfc1e223b306ca1531) commands, only your admin user will remain in the database.

