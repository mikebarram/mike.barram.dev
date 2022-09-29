---
title: "Linked servers in SQL Server"
date: "2012-05-29"
tags: ['uom']
draft: false
---

Querying across databases using linked servers should be easy:

[http://stackoverflow.com/questions/4091960/sql-server-linked-server-example-query](http://stackoverflow.com/questions/4091960/sql-server-linked-server-example-query)

but linking SQL Server  2008 (64 bit) to SQL Server 2000 (SP3 I think) results in an error:

Cannot obtain the schema rowset “DBSCHEMA\_TABLES\_INFO” for OLE DB provider “SQLNCLI10” for linked server…

To get around this the old server needs a stored procedure as follows:
```SQL
create procedure dbo.sp_tables_info_rowset_64  
  @table_name sysname,  
  @table_schema     sysname = null,  
  @table_type nvarchar(255) = null  
as  
declare @Result int set @Result = 0  
exec @Result = sp_tables_info_rowset @table_name, @table_schema, @table_type  
go
```
as described here:

[http://sqlblog.com/blogs/roman\_rehak/archive/2009/05/10/issue-with-64-bit-sql-server-using-sql-2000-linked-server.aspx](http://sqlblog.com/blogs/roman_rehak/archive/2009/05/10/issue-with-64-bit-sql-server-using-sql-2000-linked-server.aspx)

The account you’re using for the linked server also needs permission to execute the stored procedure.
