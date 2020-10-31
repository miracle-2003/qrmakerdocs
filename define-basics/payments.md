# Pricing Plans

## Subscription processors

At thee moment we have 2 subscription processors. Stripe and Paddle.com

You can manage the settings for them if you login as admin and then to got Settings-&gt; Finances. 

### Stripe

Just create account in stripe and fill you stripe credentials in  Settings-&gt; Finances.

With [Stripe Connect](https://stripe.com/connect),  you have the option, the money customers pay via ordering with online card payment, to be directly transferred  to restaurants stripe account. 

You can manage the fees you want to charge the restaurant, in the restaurant edit page.   
  
To get started with Stripe connect  
[https://dashboard.stripe.com/connect/accounts/overview](https://dashboard.stripe.com/connect/accounts/overview)



### Paddle 

QR Menu maker uses Paddle.com as payment process. It is supper easy to setup. 

Go in Paddle.com and define your pricing plans. 

As admin, when you create the plan, you will have the option to set Paddle Plan id. 

In Paddle Developer - WebHooks set the following webhook to receive subscription notification

```text
https://yoursite.com/paddle
```

{% embed url="https://vendors.paddle.com/alerts-webhooks" %}

You will also need to add paddleVendorID in .env file. You can use the .env editor to achieve this. paddleVendorID can be found in your Paddle Developer Tools -&gt; Authentication. 

[https://vendors.paddle.com/authentication](https://vendors.paddle.com/authentication)

```text
paddleVendorID=YOUR_PADDLE_VENDOR_ID
```

## **Payment currency**

QR Menu Maker supports many currencies. By default is set to **usd** currency but you can change into one of the [available currencies](https://stripe.com/docs/currencies#presentment-currencies).

```text
CASHIER_CURRENCY="usd" //usd,eur etc.
```

