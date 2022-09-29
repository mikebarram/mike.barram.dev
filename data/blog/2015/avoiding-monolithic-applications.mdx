---
title: "Avoiding monolithic applications"
date: "2015-04-10"
tags: ['uom','uom-mvc']
draft: false
---

I spend a lot (perhaps too much?) time worrying about how applications can become too big and extend beyond their original scope. When asked to create a small application that is either stand-alone or only slightly linked to other systems, it’s too tempting to just add it as an exatra section of an existing application, rather copy/re-create the infrastructure needed for it to be in its own application.

Visual Studio now provides a lot of the infrastructure, so with a few button clicks you can have an ASP.Net MVC application that’s all plumbed together but often the first thing you do is get rid of the that auto-generated stuff and it doesn’t include all of your own standard customisations. There are a few ways to implement those standard customisations:

- A class library – this is the usual way for code that needs to be included in multiple applications.
    - Version control can be an issue – if there’s a bug in the library or just an update, how do you get the new version to all users?
    - Having your own Nuget repository can help solve this, though developers may only become aware of the update when their working on the application and checking for updates. You may want a mailing list for users of the code too.
- Standardising look and feel across multiple applications – this shouldn’t be too hard to do with a Nuget that provides \_layout.cshtml razor views and standardised CSS. I haven’t tried this yet, so am copying files from application to application, which annoys me every time I do it, but hopefully I’ll have the time to look at this in future.  
    An alternative for the CSS would be to have just one copy on an assets CDN. That would need to be versioned and updated \_layouts could point to the latest version. The downside to that would be that sites may end up including multiple standard and local CSS files that then can’t be merged into one to reduce the number of downloads.
- Sometimes you want to include standard web apis in an application. A common example is an api that provides a list of staff who match a search, which is then called by a search-as-you-type component e.g. [Angularjs Typeahead](https://angular-ui.github.io/bootstrap/#/typeahead)
    - One way to do this is to include those methods in a class library. It was a surprise to fine that you can include a controller in a library and, if that class library is included in another application, then the URLs from the included library just work (unless there’s a controller in the local application with the same URL that overrides it). Because these URLs are local to the application, it is easy to lock them down so that only authenticated users have access.
    - The other, more obvious, way of providing standard web apis is to have a central site that provides them, so there’s no need to copy into each site. That works well for public apis but is more difficult for apis that require authentication. This is where [JSON Web Tokens](http://jwt.io/) and [CORS](http://www.html5rocks.com/en/tutorials/cors/) comes in.
