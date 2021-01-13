---
description: Learn how to install QR Menu Maker
---

# Installation on Shared Hosting

## Requirements

QR Menu Maker is a self-hosted web application written in PHP on top of the Laravel 5.8 framework. The followings are required to install QR Menu Maker:

* PHP Version: 7.4 or 8.0
* MySQL Version: &gt;= 5.x
* Application server: Apache, Nginx
* IMPORTANT: The script can't be installed in a subfolder. Only directly in domain or subdomain.

## Prepare to install

Installing QR Menu Maker is very easy and you'll be able to install it without any coding knowledge. The installation process included three major steps:

1. **Creating domain or subdomain**
2. **Creating a database**
3. **Uploading script files to the host**
4. **Creating environment configuration**

**Now below you can watch the video installation tutorial or you can continue with step by step.**

{% hint style="info" %}
**Warning:** The video installation tutorial doesn't include an environment explanation. You can check that in the steps below.
{% endhint %}

### Installation on Shared Hosting

Plesk / cPanel and other hosting managers are recommended. In this guide, we will use Plesk but similar should be for others.

#### 1. Create your domain or subdomain in your shared hosting

After you have created that, you will be able to access the file manager for that domain/subdomain

Delete any default files that are maybe added.

#### 2. Create a database

Create an empty database in your shared hosting and remember this credentials

* db name
* db username
* db user pass

The process of making database is something like this.

![](../.gitbook/assets/dbadd.png)

#### 3.  Upload the source code you have downloaded from CodeCanyon and unzip it

#### 4. Now navigate to the web url where your project is located

ex. mydomain.com or subdomain.mydomain.com

Click on the "Check Requirements" If some requirements is missing it will be noted out.

![](../.gitbook/assets/system.png)

Now let's check folder permissions. If some folder is noted as not writable, please check his permission. It should be 775 or 777

![](../.gitbook/assets/permissions.png)

Now we need to set up the environment. This tells Laravel how to work.

![](../.gitbook/assets/classic.png)

Select the classic text editor.

![](../.gitbook/assets/save_env%20%281%29.png)

**5. Environment Configuration**

{% hint style="info" %}
**Note:** This configuration requires many steps so we will explain this more detail.
{% endhint %}

As we already mentioned environment configuration requires many steps but just for the beginning we will need only several configurations:

* **Applications Basics** These are the first variables you will need to change.

```text
APP_NAME=Application name goes here
APP_ENV=production
APP_URL=Your website url goes here
```

* **Database Configuration** Click on the article below to continue with the database configuration.

{% page-ref page="../define-basics/database.md" %}

\*\*\*\*

When you finish with this configuration don't forget to save the .env file.

![](../.gitbook/assets/save_env.png)

Click on **Save and install**

Now the install process will begin

It will install all the necessary configurations. If some error occurs, the next screen will tell you that. Take a screenshot from it. Send to our [support chat](https://help.mobidonia.com/#QR%20Menu%20Maker).

If all goes okay, you can click on "Finish".

Now you have your own instance but the configuration is not over. Now you need to continue with the other environment configuration.

When you login as admin, you will have the option to modify and add .env values.

Click on the article below to continue with the other configuration. Everything is explained step by step.

{% page-ref page="environment-configuration.md" %}

{% hint style="danger" %}
Don't forget to do the SMTP setup. Without it, you will get error 500 on register.
{% endhint %}

Here is how to do it

{% page-ref page="../define-basics/obtain-smtp.md" %}

When you finish with the configuration we can go on the next step application usage.

Learn how to use it.

{% page-ref page="../usage/getting-started.md" %}

