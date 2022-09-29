---
title: "Using stored procedures in entity data sources"
date: "2011-02-18"
tags: ['uom', 'uom-nettiers']
draft: false
---

The normal ```<asp:SqlDataSource/>``` can use stored procedures as the select method and even for insert/update/delete commands.

netTiers will create a strongly typed data source for each table. The inserts, updates and deletes are handled automatically but there are options for which records to select. ```Get_Paged``` is the default but you can also get by any foreign key. Sometimes this isn’t enough and you want a custom filter for your entities. To do this, write a stored procedure that returns all of the columns in the base table and no other columns. The SP can have joins to other tables, so you can use those for filtering. The SP can have whatever parameters you like. Because the SP returns all of the columns of the base table, netTiers recognises that it can be used to get a list of entities and so allows it as a SelectMethod e.g.

```
<data:MyEntityDataSource ID="dMyEntityDataSource" runat="server"
  SelectMethod="MyTable\_GetByMyId\_DoSomethingSpecial"
  EnablePaging="False"
  EnableSorting="True"
  EnableDeepLoad="True"
  \>
  <Parameters>
    <asp:QueryStringParameter Name="MyId" QueryStringField="MyId" Type="String" />
  </Parameters>
</data:MyEntity>
```

The down side to this is that the stored procedure can page the records (unless you write it that way). This means that you should disable paging in the DataSource and in any linked GridView (or other control). See [previous post](https://blogs.bmh.manchester.ac.uk/nettears/2011/02/17/not-paging-with-the-entitygridview/) on the problems doing that with EntityGridViews – you have to tell it to not page in the code behind. Unless you’re having to page through a lot of records, it’s better to return them all anyway and then use the jQuery [DataTables](http://www.datatables.net/) plugin to page the records on the client side.
