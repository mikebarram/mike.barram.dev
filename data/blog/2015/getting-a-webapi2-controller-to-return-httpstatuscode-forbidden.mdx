---
title: "Getting a WebApi2 controller to return HttpStatusCode.Forbidden"
date: "2015-01-14"
tags: ['uom','uom-mvc']
draft: false
---

If your WebApi controller is checking that the user has permission to view a particular record and it turns out that they don’t then you will want to return a status of Forbidden, rather than Unauthorized as discussed here:
http://stackoverflow.com/questions/238437/why-does-authorizeattribute-redirect-to-the-login-page-for-authentication-and-au/5844884#5844884

(You might also want to override the AuthorizeAttribute class as described there)

WebApi2 controllers now return IHttpActionResult rather than HttpResponseMessage (see http://stackoverflow.com/questions/21758615/why-should-i-use-ihttpactionresult-instead-of-httpresponsemessage). It’s easy to return a result from the System.Web.Http.Results Namespace e.g. return Unauthorized();  
But the namespace doesn’t contain Forbidden, so instead use:

```C#
return ResponseMessage(new HttpResponseMessage(HttpStatusCode.Forbidden));
```
Or, more simply:

```C#
return StatusCode(HttpStatusCode.NotFound);
```