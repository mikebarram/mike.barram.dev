---
title: "NuGets of gold"
date: "2014-01-16"
tags: ['uom', 'uom-mvc', 'uom-training-hour']
draft: false
---

“NuGet is a Visual Studio extension that makes it easy to add, remove, and update libraries and tools in Visual Studio projects that use the .NET Framework.” http://docs.nuget.org/

To be as agile as possible, the projects developed by the team tend to be coded as separate .Net projects, rather than within one over-arching framework. This makes it easy, when starting a project, to copy the elements from the most similar existing project and just get on with it, without worrying about breaking existing applications. The downside to this is that bugs that are identified and fixed in one project may also need to be fixed in many other projects. In the same way, design changes (updates to templates) need to be rolled out across many sites. Updates to libraries such as jQuery or .Net need to be rolled out across many sites too but there can be an advantage in that, as testing can be done in smaller chunks before the new version can go live – plus the rule of, if it ain’t broke, don’t fix it, can be applied to the older projects that don’t have any other reason to be updated.

In an effort to consolidate the framework code that we use in all/most of our sites, I’ve investigated using NuGet. The idea is to bundle code, and even CSS files, into packages, which are hosted in a central repository. Each project then includes the packages that are needed (e.g. CAS authentication) and whenever the project is edited, Visual Studio checks to see if there is a newer version of the package. This is just like using plugins in WordPress. So, I just had to work out how to package my code…

First, you want 3 NuGet applications:

- The first is the V[isual Studio extension](http://docs.nuget.org/docs/start-here/installing-nuget) that allows you to download NuGet packages. You’ll want this anyway, to download packages such as Entity Framework, jQuery etc. It’s probably already bundled with your copy of Visual Studio
- The second is [NuGet.exe](http://nuget.org/nuget.exe), which is used to create NuGet packages. This is optional, as you can right click a solution and select “Enable NuGet Package Restore”
- The third is [NuGet Package Explorer](http://npe.codeplex.com/), which makes it easier to edit the basic package that NuGet.exe creates

To create my first NuGet package, I created a Class Library solution in Visual Studio. The class I created was nice and simple:
```C#
namespace MhsWebTeam.CasAuthentication
{

  public class TestMe
  {
    public static string GetTestString()
    {
      return "Hello from the CasAuthentication NuGet!";
    }
  }
}
```
Then I followed the instructions here: http://russellallen.info/post/2013/01/12/Complete-Idiots-Guide-to-Creating-and-publishing-a-NuGet-package.aspx

(there are also instructions here http://docs.nuget.org/docs/creating-packages/creating-and-publishing-a-package)

This gave me my first .Nupkg package file.

A folder on a network share was nominated to be the team’s repository of nuggets.

Visual Studio was then configured to point to this local repository – http://docs.nuget.org/docs/creating-packages/hosting-your-own-nuget-feeds

The local packages can then be installed in any Visual Studio project and, best of all, Visual Studio will recognise when a newer version of a package is available.

I created a new MVC project and installed the new Nuget in it. To get the Index.cshtml file to display the content from the static method I created, I added:
```C#
@MhsWebTeam.CasAuthentication.TestMe.GetTestString()
```
I could then test that the package updated sucessfully by editing the method in the original project and recompiling. Then NuGet Package Explorer was used to update the package, making sure it contained the updated dll, and the package was saved as a new file with a new version number. The new .nupkg file was copied to the local repository and, whilst I wasn’t warned that there was a new version of the package as soon as I opened the project, the update was found straight away when I right clicked on the project and selected “Manage NuGet Packages” and selected all updates. It was then a single click to update to the new version.

This is fine as a way of keeping our projects up to date with our latest dll’s but next I’ve got to work out how to package content, scripts, configurations etc.

It’s all explained here http://docs.nuget.org/docs/creating-packages/creating-and-publishing-a-package so hopefully not too hard… Editing config files with XDT stuff is just the same as you do with web.config.debug and web.config.release files.
