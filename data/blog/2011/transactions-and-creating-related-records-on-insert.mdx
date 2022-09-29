---
title: "transactions and creating related records on insert"
date: "2011-02-09"
tags: ['uom', 'uom-nettiers']
draft: false
---

After creating a record, you might want to automatically create a related child record, which uses the ID of the record you have just created. In your datasource ```<data:XyzDataSource>``` you can put in ```OnInserted="Xyz_Inserted"```:

```
<data:XyzDataSource ID="XyzDataSource" runat="server" SelectMethod="GetById" OnInserted="Xyz_Inserted">
```

```C#
protected void Xyz\_Inserted(Object sender, ObjectDataSourceStatusEventArgs e)
{
  if (e.Exception == null)
  {
    if (FormView1.CurrentMode == FormViewMode.Insert)
    {
      Xyz myXyz  = (Xyz)e.ReturnValue;
      int ID = myXyz .Id;

      // now create the child entity, set the parent id and insert it
    }
  }
}
```

The problem with this is that netTiers by default uses transactions and ```Xyz_Inserted``` is called in the middle of the transaction. So, whilst an ID has been returned for the new record, it hasn’t been committed to the database, so you can’t create the child record yet. The way around this is for the datasource to not use transactions.

```
<data:XyzDataSource ID="XyzDataSource" runat="server" EnableTransaction="false" SelectMethod="GetById" OnInserted="Xyz_Inserted">
```