---
title: "Database connections timing out in IIS 7.5 – caused by EntityTransactionModule"
date: "2011-02-08"
tags: ['uom', 'uom-nettiers']
draft: false
---

**Problem:**

After using a netTiers powered website for a while, the database connections would start to time out and you’d get a Stack Trace like:

```
at System.Data.SqlClient.SqlInternalConnection.OnError(SqlException exception, Boolean breakConnection)  
at System.Data.SqlClient.TdsParser.ThrowExceptionAndWarning(TdsParserStateObject stateObj)  
at System.Data.SqlClient.TdsParserStateObject.ReadSniError(TdsParserStateObject stateObj, UInt32 error)
```

**Solution:**

NetTiers was using an EntityTransactionModule which was incorrectly configured. It was opening database connections and not closing them (I think) and so SQL Server eventually stops allowing connections. IIS 7.5 needs the following code in the web.config to correctly configure the module.

```
<system.webServer>  
  <validation validateIntegratedModeConfiguration="false"/>  
  <modules>  
    <remove name="EntityTransactionModule"/>  
    <add name="EntityTransactionModule" type="MyApp.Web.Data.EntityTransactionModule"/>  
  </modules>  
</system.webServer>
```

I didn’t actually work this out myself, it came from the last post here [http://community.codesmithtools.com/nettiers/f/16/t/4334.aspx](http://community.codesmithtools.com/nettiers/f/16/t/4334.aspx)
