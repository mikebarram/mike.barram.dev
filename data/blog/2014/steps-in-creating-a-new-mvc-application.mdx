---
title: "Steps in creating a new MVC application"
date: "2014-03-24"
tags: ['uom', 'uom-mvc']
draft: false
---

- Create the database
- Create the project/solution in Visual Studio
    - don’t give the project the same name (in the same case) as one of the tables or the compiler will become confused between types and namespaces
    - choose MVC and optionally Web API and unit tests
    - leave authentication as Individual User Accounts
- Create an application in IIS that points to the project
- Change the Web properties for the project to use Local IIS
- Update all Nuget packages in all projects in the solution
- Add the CAS Nuget package
    - Update the web.config
        - configuration/system.web/authentication/forms
        - configuration/casClientConfig
    - AppStart\\FilterConfig.cs – add filters.Add(new System.Web.Mvc.AuthorizeAttribute());
        - See https://mikebarram.wordpress.com/2014/02/28/requiring-authentication-for-a-whole-asp-net-mvc-site/
    - Edit Controllers\\AccountController.cs – mostly copy from existing applications
    - Add Session\_Start to global.asax.cs
    - Create Views\\Shared\\NotAuthorised.cshtml
    - Create Role Provider if needed
- Web.config
    - Add ```<pages controlRenderingCompatibilityVersion=”4.0″ />``` to System.Web
- Add Nuget TinyMCE.JQuery
    - See [https://mikebarram.wordpress.com/2014/03/18/adding-wysiyyg-editors-to-text-fields-in-mvc/](https://mikebarram.wordpress.com/2014/03/18/adding-wysiyyg-editors-to-text-fields-in-mvc/)
    - Create folder Views\\Shared\\EditorTemplates
    - Create 1 line template file WYSIWYG.cshtml            ```@Html.TextArea(“”, new { @class = “wysiwyg” })```
    - Create a bundle for TinyMCE in App\_Start\\BundleConfig.cs
        
        ```
        bundles.Add(new ScriptBundle("~/bundles/tinymce").Include(
        "~/Scripts/tinymce/tinymce.min.js"));
        ```
        
- Add favicon.ico to root
- Add logo.png and user.png to Content (remember to include them in the project)
- Update Content\\site.css from an application that the new project should look like
- Create your data model
    - Don’t copy the connection string from another project as that will contain the details of the model in that project. Instead, create a new connection string for your model (you can copy the details of the server from an old connection string)
    - When editing the entity model diagram, you can change the Entity Container Name to something more friendly and that will change the name of the connection string in the web.config
    - If a connection string called “DefaultConnection” has been created in the web.config, you will want to update Models\\IdentityModels.cs to use your main connection string instead of that one – this will be the connection string that you have just set the name of in the step above.
- Start creating controllers and views…
- Auditing – if you want to automatically set the values in certain fields if they have set names (e.g. createddate):
    - Create a folder called Helpers
    - Create a partial class that overrides the SaveChanges() method of the entities (copy and modify from existing project). Method is loosely based on http://stackoverflow.com/questions/7641552/overriding-savechanges-and-setting-modifieddate-but-how-do-i-set-modifiedby
