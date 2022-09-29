---
title: "useStoredProcedure=true but still runs SELECT statements"
date: "2011-06-03"
tags: ['uom', 'uom-nettiers']
draft: false
---

.netTiers can be configured to only use stored procedures, which is a great way to reduce the possibility of the database being attacked as the user account can be given access to only execute stored procedures and not have any direct access to the tables. To do this, just set useStoredProcedure=true in the netTiers ```<providers>``` section of the web.config

If you do this, some pages (methods) will still need SELECT access to tables. By default, netTiers creates entitygridviews that use paging and so use the ```get_paged``` method, which calls the ```myTable_GetPaged``` stored procedure. This stored procedure builds a couple of SQL strings (SELECT statements) that are executed, which means that the user account needs to have access to run SELECT statements. To give SELECT access to all tables in the database, you can add the user account to the ```db_datareader``` role.
