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

