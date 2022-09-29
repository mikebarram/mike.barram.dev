---
title: "DataTables – automatic recognition of which table columns contain date/time information"
date: "2015-11-24"
tags: ['uom','uom-js']
draft: false
---

I’ve used the JavaScript [DataTables](https://datatables.net/) plug-in for jQuery a lot. It’s great for easily adding sorting to tables and lots more. It works nicely with Bootstrap too. The clunkiest thing I’ve found is trying to sort columns that contain date / time information. In the past, I used the datetables-date-sort.js plugin, which allows you to specify for each column what the data type is e.g.
```html:
<script type="text/javascript">
  $(document).ready(function () {
    $("#myTable").dataTable({
      "aLengthMenu": \[\[10, 25, 50, -1\], \[10, 25, 50, "All"\]\],
      "iDisplayLength": -1,
      "aoColumnDefs": \[
        { "bSortable": false, "aTargets": \[0\] },
        { "asSorting": \["asc", "desc"\], "aTargets": \[1, 2, 3, 4, 5, 6, 7, 8, 9, 10\] },
        { "sType": "uk-date-time", "aTargets": \[8,10\] }
      \]
    });
  });
</script>
```
That’s nice and flexible but you have to specify it for each table and, worse still, you have to (remember to) change it each time you add/remove/reorder columns.

The new “ultimate” date / time ordering plug-in described in [https://www.datatables.net/blog/2014-12-18](https://www.datatables.net/blog/2014-12-18) gets around that by recognising which columns contain date / time information. The recognition is powered by the [moment.js](http://momentjs.com/docs/#/displaying/) library. The only customisation that you have to do is specify which date / time formats you’ll be using, but you’ll hopefully standardise them into just a handful across the whole site anyway.

Now I have a script like this, which is written just once and called by every page:

```html:
<script type="text/javascript">
  $(document).ready(function () {
    $.fn.dataTable.moment('DD/MM/YYYY');
    $.fn.dataTable.moment('DD/MM/YYYY HH:mm:SS');
    $('.mhsStandardDataTable.mhsNoPaging').DataTable({
      paging: false
    });
    $('.mhsStandardDataTable:not(.mhsNoPaging)').dataTable({
      paging: true,
      "aLengthMenu": \[\[10, 25, 50, -1\], \[10, 25, 50, "All"\]\],
      "iDisplayLength": -1
    });
  });
</script>
```

To turn any table into a DataTable, I just add the class mhsStandardDataTable. Sometimes I don’t want paging (usually if I’m expecting no more than 20 rows), so I can add the class mhsNoPaging and that removes some of the clutter.

In the example above, I’ve restricted myself to just 3 date / time formats. The more verbose formats, with day or month spelt out, are great for making a date really clear and unambiguous but I never use them in tables.
