# Pricing Plans

## Subscription processors

At thee moment we have 2 subscription processors. Stripe and Paddle.com

You can manage the settings for them if you login as admin and then to got Settings-&gt; Finances. 

### Stripe

Just create account in stripe and fill you stripe credentials in  Settings-&gt; Finances.

### Paddle 

QR Menu maker uses Paddle.com as payment process. It is supper easy to setup. 

Go in Paddle.com and define your pricing plans. 

As admin, when you create the plan, you will have the option to set Paddle Plan id. 

In Paddle Developer - WebHooks set the following web-hook to receive subscription notification

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

QR Menu Maker supports many currencies. By default is set to **usd** currency but you can change into one of the [available currencies](https://stripe.com/docs/currencies#presentment-currencies). You can manage the currencies in Setting -&gt; Localization.

```text
CASHIER_CURRENCY="usd" //usd,eur etc.
```

