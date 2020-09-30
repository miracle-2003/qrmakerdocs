# Changelog

## 1.5.5 - 2020-09-30

### Improvements

* Custom CSS and JS for frontend and backed set from the admin
* Landing page into separate files for easier update
* Gravatar image corrections

### How to update

Just log in as admin, and you should see "New Update 1.5.5". Click on the button. 

{% hint style="warning" %}
This update will change your landing page. But your landing.blade.php file is not modified. Landing now uses home.blade.php and uses separate files to show content. We did this for easier future updates.   
  
The content of the landing page is now in resources/views/qrsaas/partials  
  
To show your old landing, just add .env variable  
QR\_LANDING=landing
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

