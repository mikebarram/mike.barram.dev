---
title: "EntityFramework Reverse POCO Generator and Views"
date: "2014-09-20"
tags: ['uom', 'uom-mvc']
draft: false
---

EntityFramework’s own tool to generate a model from a database is slow and buggy. It’s particularly a problem if you update your database (change table names, field names etc.).

[EntityFramework Reverse POCO Generator](http://visualstudiogallery.msdn.microsoft.com/ee4fcff9-0c4c-4179-afd9-7a2fb90f5838) is a great, lightweight replacement – it’s fast, configurable and just works. Also, the entities created can be the same as those created by the built in tool, so it is possible to switch to it part way through developing a project.

The only problem I’ve encountered is where I need to create an entity (read-only) from a view. In this case a view on a table in a different database. Because it can’t read the schema of the underlying table, it can get data types and nullability wrong. To help Reverse POCO Generator get it right, you can use CAST to show that the field really is whatever data type it is and you can also use ```ISNULL([non-null-field],0)``` to show that the field will never be null. A problem with using ISNULL is that Reverse POCO Generator will use non-null fields to create a primary key, so you may want to do the opposite and use ```NULLIF([non-null-non-key-field],-1)```. This is all better explained here:

http://girlfromoutofthisworld.com/entity-framework-and-setting-primary-keys-on-views/
