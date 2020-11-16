# Pricing Plans

## Subscription processors

At the moment we have 2 subscription processors. Stripe and Paddle.com

You can manage the settings for them if you login as admin and then to got Settings-&gt; Finances. 

### Stripe

Just create an account in stripe and fill your stripe credentials in  Settings-&gt; Finances.

One common mistake is to use plan\_id instead of price\_id. So you should use the price\_id from Stripe. As you can see in the image.

![](../.gitbook/assets/plans.png)

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

