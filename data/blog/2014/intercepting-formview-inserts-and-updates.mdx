---
title: "Intercepting FormView inserts and updates"
date: "2014-01-27"
tags: ['uom']
draft: false
---

Our FormViews in ASP.Net web forms tend to contain user controls in the templates.

If you want to want to intercept the insert or update events, you end up with something like:
```C#
protected void FormView1_ItemUpdating(object sender, FormViewUpdateEventArgs e)  
{

}
```

But how do you access the values in the user control? We’ve often had code like this:

```C#
TextBox tReviewerName = (TextBox)FormView1.Row.FindControl("dataReviewerName");
```
which is OK to get the value from that field if you want to code your own updates/inserts but you can’t (I think) write back to that field in time for the update to pass that new value back to the database.

The better/correct way to update the data is like so:
```C#
protected void FormView1_ItemUpdating(object sender, FormViewUpdateEventArgs e)  
{
  string sOut = e.NewValues["ReviewerName"].ToString();
  sOut = sOut.Replace("rude word", "kitten");
  e.NewValues["ReviewerName"] = sOut;
}
```