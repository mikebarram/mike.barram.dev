---
title: "RewriteRules in .htaccess files that run after a set date/time"
date: "2016-07-27"
tags: ["uom"]
draft: false
---

If you’re going to launch a website out of hours and want an old site that uses Apache to redirect to the new site, you can set a list of rewrite rules to run after a certain time. The trick is to write a condition that makes a rule run until the launch date and that rule skips the new rules. After the launch date, the rule doesn’t run, so the new rules aren’t skipped:

```
# Turn on the rewriting engine
RewriteEngine On

# if the date/time is BEFORE 7:30am on 1st August 2016, the condition is met, so the first rewrite rule executes and skips the next 7 rules.
# if the date/time is AFTER 7:30am on 1st August 2016, the condition is not met, so the first rule does not run and therefore the following rules are run (until a match is found, which the last rule is guaranteed to do)
# RewriteRules that match a URL are best sorted in reverse order to be sure that the most specific match is found first

RewriteCond %{TIME_YEAR}%{TIME_MON}%{TIME_DAY}%{TIME_HOUR}%{TIME_MIN} <201608010730
RewriteRule .* – [S=7]
RewriteRule ^section2/subsection2 http://www.newsite.com/section2/subsection2 [NC,L,R=301]
RewriteRule ^section2/subsection1 http://www.newsite.com/section2/subsection1 [NC,L,R=301]
RewriteRule ^section2 http://www.newsite.com/section2 [NC,L,R=301]
RewriteRule ^section1/subsection2 http://www.newsite.com/section1/subsection2 [NC,L,R=301]
RewriteRule ^section1/subsection1 http://www.newsite.com/section1/subsection1 [NC,L,R=301]
RewriteRule ^section1 http://www.newsite.com/section1 [NC,L,R=301]
RewriteRule .* http://www.newsite.com/ [NC,L,R=301]
```
