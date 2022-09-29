---
title: "Requiring authentication for a whole ASP.Net MVC site"
date: "2014-02-28"
tags: ['uom', 'uom-mvc'] 
draft: false
---

This is easy from ASP.NET MVC 4 onwards:  
http://blogs.msdn.com/b/rickandy/archive/2012/03/23/securing-your-asp-net-mvc-4-app-and-the-new-allowanonymous-attribute.aspx

You can register a filter that will require users to be authenticated to access all controllers

```C#
public static void RegisterGlobalFilters(GlobalFilterCollection filters)
{
    filters.Add(new HandleErrorAttribute());
    filters.Add(new System.Web.Mvc.AuthorizeAttribute());
}
```

but then they won’t be able to access to the Login controller, so you simply add the \[AllowAnonymous\] attribute to that controller:

```C#
[AllowAnonymous]
public ActionResult Login(string returnUrl)

[HttpPost]
[AllowAnonymous]
[ValidateAntiForgeryToken]
public ActionResult Login(LoginModel model, string returnUrl)
```
