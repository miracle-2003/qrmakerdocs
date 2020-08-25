# Pricing Plans

QR Menu maker uses Paddle.com as payment process. It is supper easy to setup. 

Go in Paddle.com and define your pricing plans. 

As admin, when you create the plan, you will have the option to set Paddle Plan id. 

In Paddle Developer - WebHooks set the following webhook to receive subscription notification

```text
https://yoursite.com/paddle
```

{% embed url="https://vendors.paddle.com/alerts-webhooks" %}



## **Payment currency**

QR Menu Maker supports many currencies. By default is set to **usd** currency but you can change into one of the [available currencies](https://stripe.com/docs/currencies#presentment-currencies).

```text
CASHIER_CURRENCY="usd" //usd,eur etc.
```

