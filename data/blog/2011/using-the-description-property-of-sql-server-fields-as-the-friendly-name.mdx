---
title: "Using the description property of SQL Server fields as the friendly name"
date: "2011-03-17"
tags: ['uom', 'uom-nettiers']
---

SQL Server allows each field in the database to have a description, so this description seems like the most useful place to put friendly names for fields that will appear on a netTiers generated admin page.

When netTiers first runs, a config file is generated as specified in 01 MappingFile  
This XML file lists all of the tables and for each table it lists all of the fields e.g.
```
<Column Id="title" CSType="System.String" PropertyName="Title" FieldName="_title" FriendlyName="Title" IncludeInOutput="true" />
```

netTiers will automatically convert the database field name of "title" to a FriendlyName of "Title"  
It’s quite clever too and will convert a field name of ```"title_or_salutation"``` to a FriendlyName of ```"Title Or Salutation"```

You can just modify the FriendlyNames in the config file (e.g. change it to FriendlyName="Title or salutation"), regenerate the project and those modified FriendlyNames will be used as labels for fields in the admin pages. That doesn’t work well when your database structure keeps changing as new fields won’t be added to the config file.

So, the solution is for netTiers to recreate the config file each time the project is regenerated but for the FriendlyNames to come from the description property in the database.

The following change to the netTiers script will do this:

SchemaMappingNetTiersMapInstance.Internal.cst

change as described here http://community.codesmithtools.com/nettiers/f/34/p/9968/37042.aspx#37042

**Line 22** change
```
<Table Id="<%= table.Name %>" EntityName="<%=GetClassName(table)%>" Owner="<%=GetOwnerName(table)%>" PropertyName="<%= GetPropertyName(table) %>" FieldName="<%= GetFieldName(table) %>" FriendlyName="<%= GetFriendlyName(table) %>" IncludeInOutput="true">
```
to
```
<Table Id="<%= table.Name %>" EntityName="<%=GetClassName(table)%>" Owner="<%=GetOwnerName(table)%>" PropertyName="<%= GetPropertyName(table) %>" FieldName="<%= GetFieldName(table) %>" FriendlyName="<%= ((table.ExtendedProperties["MS_Description"\]==null)||(table.ExtendedProperties["MS_Description"\].Value.ToString().Length==0))?GetFriendlyName(table):table.ExtendedProperties["MS_Description"\].Value.ToString() %>" IncludeInOutput="true">
```
**Line 25** change
```
<Column Id="<%= column.Name %>" CSType="<%= GetCSType(column) %>" PropertyName="<%= GetPropertyName(column) %>" FieldName="<%= GetFieldName(column) %>" FriendlyName="<%= GetFriendlyName(column) %>" IncludeInOutput="true" />
```
to
```
<Column Id="<%= column.Name %>" CSType="<%= GetCSType(column) %>" PropertyName="<%= GetPropertyName(column) %>" FieldName="<%= GetFieldName(column) %>" FriendlyName="<%= ((column.ExtendedProperties["MS_Description"\]==null)||(column.ExtendedProperties["MS_Description"\].Value.ToString().Length==0))?GetFriendlyName(column):column.ExtendedProperties["MS_Description"\].Value.ToString() %>" IncludeInOutput="true" />
```
**Line 36** change
```
<View Id="<%=view.Name%>" EntityName="<%=GetClassName(view)%>" Owner="<%=GetOwnerName(view)%>" PropertyName="<%= GetPropertyName(view) %>" FieldName="<%= GetFieldName(view) %>" FriendlyName="<%= GetFriendlyName(view) %>" IncludeInOutput="true">
```
to
```
<View Id="<%=view.Name%>" EntityName="<%=GetClassName(view)%>" Owner="<%=GetOwnerName(view)%>" PropertyName="<%= GetPropertyName(view) %>" FieldName="<%= GetFieldName(view) %>" FriendlyName="<%= ((view.ExtendedProperties["MS_Description"\]==null)||(view.ExtendedProperties["MS_Description"\].Value.ToString().Length==0))?GetFriendlyName(view):view.ExtendedProperties["MS_Description"\].Value.ToString() %>" IncludeInOutput="true">
```
**Line 40** change
```
<Column Id="<%= column.Name %>" CSType="<%= GetCSType(column) %>" PropertyName="<%= GetPropertyName(column) %>" FieldName="<%= GetFieldName(column) %>" FriendlyName="<%= GetFriendlyName(column) %>" IncludeInOutput="true" />
```
to
```
<Column Id="<%= column.Name %>" CSType="<%= GetCSType(column) %>" PropertyName="<%= GetPropertyName(column) %>" FieldName="<%= GetFieldName(column) %>" FriendlyName="<%= ((column.ExtendedProperties["MS_Description"\]==null)||(column.ExtendedProperties["MS_Description"\].Value.ToString().Length==0))?GetFriendlyName(column):column.ExtendedProperties["MS_Description"\].Value.ToString() %>" IncludeInOutput="true" />
```