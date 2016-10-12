---
layout: post
title: Finally, No More Invalid Credit Cards
date: 2016-05-06 16:27:31
heroimage: images/swiss1.jpg
published: true
---

Today, we are excited to announce a new feature allowing you to quickly validate credit card at any time.

From time to time we get asked if there is a way to check if a credit card is still valid.Especially in the hospitality sector, where credit cards are often used only couple months after they were initially stored, invalid credit cards can become big problems. For instance, if a customer booked a hotel room and never shows up, the property manager wants to charge the no-show fee. By then,

> We extended our a neat XML interface allowing you to **quickly validate a credit card at any time.**


Learn how you can use it:
---

* Grab the token of the credit card you want to check.
* Send the following XML request to our XML_Authorize.jsp Endpoint:
{% highlight xml linenos %}
<?xml version="1.0" encoding="UTF-8" ?>
        <authorizationService version="2">
            <body merchantId="1000011011">
                <transaction refno="1234987">
                    <request>
                        <amount>0</amount>
                        <currency>CHF</currency>
                        <aliasCC>70323122544331174</aliasCC>
                        <expm>12</expm>
                        <expy>15</expy>
                        <sign>30916165706580013</sign>
                    </request>
                </transaction>
            </body>
        </authorizationService>
{% endhighlight %}



There is no clever design philosophy to talk about, I tried to find something to work with, and 'scribble' came to my mind. This theme uses Open Sans powered by Google Web Fonts, and was written in plain HTML, SCSS & CoffeeScript, though .scss & .coffee files wouldn't be included in the theme.

The theme is mobile optimised but I did not check browser compatibility. It looks great in Chrome, Safari and Firefox though.

<a href="https://www.pci-proxy.com/#/signup" target="_blank" class="big-button blue">Get your free PCI Proxy test account &hearts;</a>

---
