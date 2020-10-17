# Environment configuration

All of the configuration variables for the QR Menu Maker project are stored in the **`.env`** file.

QR Menu Maker installation, the root directory of your application will contain a **`.env.example`** file. You will need to rename it manually to **`.env`**

List of all custom environment variables QR Menu Maker uses. We will see them one by one.

{% hint style="info" %}
Remove the comments // when you add some environment variable
{% endhint %}

### **1. Database**

{% page-ref page="../define-basics/database.md" %}

### **2. Mail server**

{% page-ref page="../define-basics/obtain-smtp.md" %}

### **3. Localization and Time format**

{% page-ref page="../define-basics/localization.md" %}

### **4. Pricing plans**

{% page-ref page="../define-basics/payments.md" %}

### 5. Google Analytics

From version 1.2 we enable tracks and reports website traffic using Google Analytics. This is optionally and if you want to enable on your site you need to create a Google Analytics code.

{% page-ref page="../define-basics/google-analytics.md" %}

### 6. Google ReCaptcha \( since 1.5.8 \)

To protect your site from spammy form submits we have implemented Invisible ReCaptcha. ReCaptcha.

{% hint style="success" %}
We are using this [plugin](https://laravel-recaptcha-docs.biscolab.com/docs/intro) for Laravel.   
  
To enable it on the registration form,  you have to create your own API keys [here](https://www.google.com/recaptcha/admin).  
reCAPTCHA type:**v2 Invisible**  
  
Then you need to enter thous keys in .env  
  
in your .env file

RECAPTCHA\_SITE\_KEY=YOUR\_API\_SITE\_KEY RECAPTCHA\_SECRET\_KEY=YOUR\_API\_SECRET\_KEY
{% endhint %}

### 7. Frontend list of languages \( since 1.5.8 \)

{% hint style="success" %}
To modify the list of available language add new .env variable

FRONT\_LANGUAGES=EN,English,FR,French

To hide the language selector, just declare one language
{% endhint %}

### 8. Subdomain

When you run your site in a subdomain, you need to declare that subdomain in your .env file. This is needed to be clarified since this project can be used with subdomains for each restaurant.

```text
IGNORE_SUBDOMAINS="www,yoursubdomain,anothersubdomain"
```

### 9. Import from CSV

QR Menu Maker also supports integration and working with excel files.

### 10. Additional variables

There are also a few variables that for now only we will mention and later we will explain more about them.

If you want to skip adding the demo data that you will find on the [demo version](https://QR%20Menu%20Maker.site/) you can make that by adding a variable in the configuration.

```text
DEMO_DATA=false //By default it's true, if false the data won't be added
```

Additionally, if you add the demo data in the process of installation later you can delete manually but maybe you will have some conflicts during this process.

{% embed url="https://mobidonia.gitbook.io/qr-menu-maker/changelog/faq\#how-to-delete-the-demo-data" %}

