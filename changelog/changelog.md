# Changelog

## 1.7.8 - 2020-11-08

### Improvements

* Dine-in / Takeaway when making an order
* Option to not offer a free plan \( set FREE\_PLAN\_ID to 0 \)
* Images for a menu item, are no longer required
* Fixes on working with the variants
* Fixes on registering customer visit by the customer

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.8. Click on the button. 

## 1.7.7 - 2020-11-01

This is a combined update from 1.7.3 till 1.7.7

### Improvements

* Change landing page images via settings

### Fixes

* Stripe system status check
* REcaptcha fix
* Plan removing fixes
* Fixes for managing options and variants

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.X. Click on the button. 



## 1.7.3 - 2020-10-28 

{% embed url="https://www.loom.com/share/15cc92bffca0416da783972f55bbce79" %}

This is combined update from 1.5.8 till 1.7.3

### Improvements

* Tables and area management
* Local order \( Continuous orders and online card payments \)
* Orders \| Report and live orders
* Customer log
* Subscribe via stripe
* Manually assign restaurant to pricing plan

{% hint style="info" %}
This update introduces Stripe as default way for accepting subscriptions. To enable it, you need to register stripe account, and create product in it. When you create the pricing plans, you will need to enter Stripe pricing\_id for each plan.   
  
New variables in .env  
  
ENABLE\_STRIPE\_CONNECT=true   
ENABLE\_FINANCES\_OWNER=true  
ENABLE\_FINANCES\_ADMIN=true  
ENABLE\_STRIPE=true  
STRIPE\_KEY='pk\_test\_XXXXXXXXXXXXXX'  
STRIPE\_SECRET='sk\_test\_XXXXXXXXXXXXXXX',  
SUBSCRIPTION\_PROCESSOR=Stripe  
QRSAAS\_DISABLE\_ODERING=false
{% endhint %}

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.3. Click on the button. 

## 1.5.8 - 2020-10-17

This is a combined update from 1.5.6 \| 1.5.7 and 1.5.8

### Improvements

* Google ReCaptcha added
* Better Favicon generation
* Better frontend language manager
* Limit plan fix
* Better URL route for restaurant edit
* Other small bug fixes

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.5.5". Click on the button. 



{% hint style="success" %}
This update changes the config for the frontend languages

To modify the list of available language add new .env variable

FRONT\_LANGUAGES=EN,English,FR,French
{% endhint %}

{% hint style="success" %}
In this update we introduced the Google Recaptcha.   
We are using this [plugin](https://laravel-recaptcha-docs.biscolab.com/docs/intro) for Laravel. And we have implemented the invisible recaptcha.  
  
To enable it on the registration form,  you have to create your own API keys [here](https://www.google.com/recaptcha/admin).  
reCAPTCHA type:**v2 Invisible**  
  
Then you need to enter thous keys in .env  
  
in your .env file

RECAPTCHA\_SITE\_KEY=YOUR\_API\_SITE\_KEY RECAPTCHA\_SECRET\_KEY=YOUR\_API\_SECRET\_KEY
{% endhint %}

## 1.5.5 - 2020-09-30

### Improvements

* System setup status and better error handling
* Translation management
* Custom CSS and JS for frontend and backed set from the admin
* Landing page into separate files for easier update
* Gravatar image corrections

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.5.5". Click on the button. 

{% hint style="warning" %}
This update will change your landing page. But your landing.blade.php file is not modified. Landing now uses home.blade.php and uses separate files to show content. We did this for easier future updates.   
  
The content of the landing page is now in resources/views/qrsaas/partials  
  
To show your old landing, just add .env variable  
QR\_LANDING=landing

To modify the list of available language add new .env variable

LANGUAGES={ "EN":"English","FR":"French"}
{% endhint %}

## 1.5.4 - 2020-09-29 \( test update \)

{% hint style="info" %}
This is the first incremental update that can be done via the 1Click Update button.   
If you receive an error like HOME ACTION NOT ALLOWED it is because you are logged in as admin, but the admin ID is not 1.  Open config/laraupdater.php and at the bottom modify the variable allow\_users\_id to have the admin ID, or set to false to accept all admins. 
{% endhint %}

### **Fixes**

* Paddle vendor id correct setup

## 1.5.3 - 2020-09-29

### Improvements

* One-Click update button 
* Favicon change setup from admin settings
* Removed more unnecessary fields in admin
* Fixes on the  menu on mobile phone
* Spelling mistakes corrected on landing
* Removed 40 00+ Unnecessary developer files
* Plan limit:  now prevent the user to add new items in the menu if the limit is reached

### How to update

Follow the standard update procedure

{% page-ref page="updating-shared-hosting.md" %}

From this version on, when there is a new update, log in as admin, and you will see a blue card on left, indicating that there is an update you can apply. 

{% hint style="warning" %}
This update brings updates on the landing page. if you have modified, you may want to back it before updating. 
{% endhint %}



## 1.5.2 - 2020-09-24 \( [Video](https://youtu.be/gZ7WGhdOq5I) \)

### Fixes

* Better documentation 
* Option to add / change the print templates provided
* Option to translate the QR Maker page for restaurants
* Removed unnecessary fields and options for admin
* Categories Filter fixed
* Removed wizard option from the install screen
* Option to disable landing page DISABLE\_LANDING in .env

### How to update

Follow the standard update procedure

{% page-ref page="updating-shared-hosting.md" %}

Or, here is the list of file modified, so you can change them one by one if you prefer. 

{% embed url="https://1drv.ms/u/s!AqVDdjJrM4dRhoV2HokQUTkzOTlIqg" %}



## 1.5.1 - 2020-09-19

### Initial Version

