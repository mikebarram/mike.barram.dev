---
title: "NetTiers EntityGridView Deepload display readonly lookup"
date: "2011-02-08"
tags: ['uom', 'uom-nettiers']
draft: false
---

If you need your netTiers gridview (EntityGridView) to have a column that just displays a read only value from a lookup table then the data source will need to deepload but ```<asp:BoundField>``` won’t be able to access the lookup value. NetTiers’ own controls are only dropdowns, hyperlinks and radiobuttons, so to display the lookup value (rather than the ID), you need to add a template field

```
<asp:TemplateField>  
  <ItemTemplate>  
    <%# Eval("ApplicIdSource.Applic")%>  
  </ItemTemplate>  
</asp:TemplateField>
```

as described here:

[http://community.codesmithtools.com/nettiers/f/16/p/7121/27053.aspx](http://community.codesmithtools.com/nettiers/f/16/p/7121/27053.aspx)

An alternative to this is to use a <data:HyperLinkField/> field, use CSS to stop it looking like a hyperlink and don’t let it navigate anywhere:

```
<data:HyperLinkField ControlStyle-CssClass="table-hyperlink-nofollow" HeaderText="Body part" DataNavigateUrlFormatString="#" DataNavigateUrlFields="Bodypartid" DataContainer="BodypartidSource" DataTextField="Bodypartdescription" />
```

The first method is probably the better way.
