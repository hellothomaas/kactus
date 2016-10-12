---
layout: post
title: "Official Markdown Testfile"
date: 2016-10-06 15:27:31
description: "That's about all Markdown Features"
author: "Thomas S. Willenborg"
authorPic: "thomas.jpg"
authorUrl: "https://twitter.com/tswillenborg"
authorTwitter: "tswillenborg"
tags: [random, diary, school]
---

# Header 1
## Header 2
### Header 3
#### Header 4

You are a middle office that receives booking information on behalf of your clients.

> Travel agencies use your software to drop new bookings. At some point, they will enter the customers’ payment data in your software. In order `<a href>` to minimize your PCI scope, this payment data should be added without touching your server.

We support different approaches how you can securely collect the customers´ credit card details. Start with a simple HTML `<a href>` tag:

---

### Buttons

<a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp?merchantId=1100004624&refno=pci-proxy-redirect&amount=1&currency=CHF&theme=DT2015&uppAliasOnly=yes" target="_blank" class="big-button gray">Collect Credit Card</a>
<a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp?merchantId=1100004624&refno=pci-proxy-redirect&amount=1&currency=CHF&theme=DT2015&uppAliasOnly=yes" target="_blank" class="big-button red">Collect Credit Card</a>
<a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp?merchantId=1100004624&refno=pci-proxy-redirect&amount=1&currency=CHF&theme=DT2015&uppAliasOnly=yes" target="_blank" class="big-button blue">Collect Credit Card</a>
<a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp?merchantId=1100004624&refno=pci-proxy-redirect&amount=1&currency=CHF&theme=DT2015&uppAliasOnly=yes" target="_blank" class="big-button green">Collect Credit Card</a>

---

### Tables

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

---

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

---

### Syntax highlighting

{% highlight html %}
<a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp
            ?merchantId=1100004624
            &refno=pci-proxy-redirect
            &amount=1
            &currency=CHF
            &theme=DT2015
            &uppAliasOnly=yes">Collect payment data</a>
{% endhighlight %}

PCI Proxy supports a varienty of [different approaches for you to collect the payment data][1]. Your server will never get in touch with sensitive card data which reduces your PCI scope immediately.

 The most common approach is to submit data directly from your software using our [payment pages][2]. Another option is [pay-by-email][3] where temporary payment links are issued that can be emailed to customers to let them enter their payment details by themselves.

 {% highlight ruby %}
 <a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp
             ?merchantId=1100004624
             &refno=pci-proxy-redirect
             &amount=1
             &currency=CHF
             &theme=DT2015
             &uppAliasOnly=yes">Collect payment data</a>
 {% endhighlight %}

*On behalf of your clients you want to process the booking or transact with different endpoints (e.g. Expedia, Stripe, TUI, Lufthansa, etc.).*

 PCI Proxy allows you to [forward vaulted payment data][4] to PCI compliant third parties.



1. List with code

  ```html
  not highlighted
  multi line
  ```
2. List with code{% highlight javascript %}
var dom = document.getElementById('boom')
console.log(dom);
{% endhighlight %}

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim.

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.

{% highlight ruby %}
<a href="https://pilot.datatrans.biz/upp/jsp/upStart.jsp
            ?merchantId=1100004624
            &refno=pci-proxy-redirect
            &amount=1
            &currency=CHF
            &theme=DT2015
            &uppAliasOnly=yes">Collect payment data</a>
{% endhighlight %}

[1]: collect_payment_data.html
[2]: website-application.html
[3]: https://www.datatrans.ch/en/offer/special-solutions/pay-by-e-mail
[4]: forward.html

---

1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses
