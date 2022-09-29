---
title: "Multiline Text Editor in MVC"
date: "2014-02-27"
tags: ['uom', 'uom-mvc']
draft: false
---

In ASP.Net MVC, it’s so easy to create an entity data model and generate controllers and views for each entity. You can create lots of pages for editing your data just by clicking buttons…

A downside is that the generated code doesn’t know the the difference between a small string and a large one, so you get the same small text input box to edit all strings.

In your razor view, that’s created by

```C#
@Html.EditorFor(model => model.YourTextField)
```

This http://stackoverflow.com/questions/4927003/asp-net-mvc3-textarea-with-html-editorfor explains that you can set a [`[DataType]`](http://msdn.microsoft.com/en-us/library/system.componentmodel.dataannotations.datatypeattribute.aspx) attribute on the view model e.g.

```C#
public class MyViewModel
{
    [DataType(DataType.MultilineText)]
    public string YourTextField{ get; set; }
}
```

But, if your view model has been generated, you can’t edit it (or at least your changes will be reverted when you re-generate the model from the database).

Fortunately, this http://stackoverflow.com/questions/16736494/add-data-annotations-to-a-class-generated-by-entity-framework explains how to create a second partial class that lets you set the data attributes

```C#
namespace SameNamespace.Models
{
	[MetadataType(typeof(YourClassMetaData))]
	public partial class YourClass
	{
	}

	public class YourClassMetaData
	{
		[DataType(DataType.MultilineText)]
		public string YourTextField { get; set; }
	}
}
```

If you’re not displaying data directly from a model but from a view model, then the field in the view model will need the data attribute.

At the same time, if the text box is for HTML, you might want to add the \[AllowHtml\] attribute to the property. If you then get the error “A potentially dangerous Request.Form value was detected”, you may need to set this in the web.config:

A simpler way, but one that won’t globally affect the way the field is displayed, is to use:

```C#
@Html.TextAreaFor(model => model.YourTextField, new { cols = 80, @rows = 15 })
```
