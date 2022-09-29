---
title: "HTTP Referer / Referrer and HTTPS"
date: "2015-03-27"
tags: ['uom']
draft: false
---

The rule for whether the HTTP referrer (incorrectly spelt in the original spec, so forever incorrectly spelt in headers) is sent along with a request has always been a bit odd. If the referring site uses https, the referrer isn’t sent, unless the site linked too also uses https. It isn’t sent because the originating URL may contain sensitive information but the browser happily sends the sensitive URL to any other site if it uses https.

Now, there is a meta tag you can use that tells browsers whether or not to send the referrer. The options are Never, Origin (only the domain name is sent), Default (same as without the tag), Always. If you’re not worried about other sites knowing your site exists and links to their site, 
```<meta name="referrer" content="origin">``` seems the best option for sites using htttps.

This has been implemented in Chrome, Safari and [recently in Firefox](https://bugzilla.mozilla.org/show_bug.cgi?id=704320)

There’s a better description of this here:  
http://smerity.com/articles/2013/where\_did\_all\_the\_http\_referrers\_go.html

It looks like the options are being changed:  
http://w3c.github.io/webappsec/specs/referrer-policy/#referrer-policy-delivery-meta

They’re now:

- no-referrer
- origin
- no-referrer-when-downgrade
- origin-when-crossorigin
- unsafe-url

origin-when-crossorigin sounds like a better option for most intranets, as one page in the intranet can get the full referrer when linked to from another, but external sites (whether using https or not) will just get the domain name. At the moment (27th March 2015), I think Firefox supports these latest values but Chrome doesn’t, so it’s better to use origin.

As well as a page-wide meta tag, you can also set a referrer attribute on the 
```<a>, <area>, <img> or <iframe>``` 
elements:  
http://w3c.github.io/webappsec/specs/referrer-policy/#referrer-policy-delivery-referrer-attribute
