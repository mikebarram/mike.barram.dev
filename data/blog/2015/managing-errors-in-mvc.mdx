---
title: "Managing errors in MVC"
date: "2015-01-14"
tags: ['uom','uom-mvc']
draft: false
---

## Error logging

Elmah seems to be the most popular tool for error logging but the Elmah website doesn’t have much up to date information on how to get started. To get Elmah installed, secured and logging to somewhere more permanent than keeping the log in-memory, follow this guide: http://www.erikojebo.se/Code/Details/607

## Error handling

Elmah just logs error, it doesn’t help the user. So you also need to handle the errors, which this article covers nicely:  
https://www.simple-talk.com/dotnet/asp.net/handling-errors-effectively-in-asp.net-mvc/

In the web.config:
```html:
    <httpErrors errorMode\="Custom" existingResponse\="Replace"\>
      <remove statusCode\="403" />
      <error statusCode\="403" path\="/WorkloadPlanner/Error/403" responseMode\="ExecuteURL" />
      <remove statusCode\="404" />
      <error statusCode\="404" path\="/WorkloadPlanner/Error/404" responseMode\="ExecuteURL" />
      <remove statusCode\="500" />
      <error statusCode\="500" path\="/WorkloadPlanner/Error/500" responseMode\="ExecuteURL" />
    </httpErrors\>
```
Then an "error" controller:
```C#
\[RoutePrefix("error")\]
\[Route("{action=index}")\]
public class ErrorController : Controller
{
    // GET: Error
    \[Route("{StatusCode}")\]
    public ActionResult Index(int? StatusCode)
    {
        if (null == StatusCode)
        {
            return View("Exceptions/Unknown");
        }
 
        Response.StatusCode = (int)StatusCode;
        return View("Exceptions/" + StatusCode.ToString());
 
    }
}
```
Then, for each exception, a very simple view with the appropriate error message.

The advantage of this is that it allows for code in the controller e.g. switch(StatusCode) and more verbose error messages, and even pictures, in the views.

## Handling requests where the user is allowed to access the “page” (i.e. method in the controller) but not for the specified parameter(s).

In other words, the user doesn’t have permission to view/edit/delete a record

Sometimes you want the user to be able to try and do something they shouldn’t, so that they can see that it’s possible and that they just need to ask for access. In those cases, I’ll do a permission check and if they haven’t got permission, the controller will return a custom view that explains the problem and how to request access. At the same time, without throwing an error, I’d like to return the HTTP status code 403 Forbidden. This explains why 403 rather than 401 http://stackoverflow.com/questions/3297048/403-forbidden-vs-401-unauthorized-http-responses.

Other times, the user really should have found their way to the URL, so I want to log the log the Error to Elmah and then return a view and 403 status code as above.

As with the generic errors above, for each message that I want to return to the user, I’ve created a view.

Then I’ve created a helper class that gets the name of the view and sets the status code and whether to log errors:

```C#:
public static class ExceptionHelper
{
    public enum ExceptionName { NotOwnWorkload, NotReportViewerForGroup, WorkloadNotRecorded };
 
    /// <summary>
    /// Gets the name of the view related to the exception name entered.
    /// Sets the StatusCode of the response as requested or to the default for the specified exception.
    /// Logs the exception if specified or if that's the default behavious for the exception.
    /// </summary>
    /// <param name="ExceptionName"\>Name of the exception.</param>
    /// <param name="StatusCode"\>The status code.</param>
    /// <param name="LogException"\>The log exception.</param>
    /// <returns></returns>
    public static string GetViewName(ExceptionName ExceptionName, HttpStatusCode? StatusCode = null, bool? LogException = null)
    {
        // set a default return status code
        HttpStatusCode returnStatusCode = HttpStatusCode.BadRequest;
 
        if (null == StatusCode)
        {
            // use the default for he ExceptionName to decide
            switch (ExceptionName)
            {
                case ExceptionName.NotOwnWorkload:
                    returnStatusCode = HttpStatusCode.Forbidden;
                    break;
                case ExceptionName.NotReportViewerForGroup:
                    returnStatusCode = HttpStatusCode.Forbidden;
                    break;
                case ExceptionName.WorkloadNotRecorded:
                    returnStatusCode = HttpStatusCode.OK;
                    break;
                default:
                    returnStatusCode = HttpStatusCode.BadRequest;
                    break;
            }
        }
        else
        {
            // StatusCode not null so convert to Boolean
            returnStatusCode = (HttpStatusCode)StatusCode;
        }
        HttpContext.Current.Response.StatusCode = (int)returnStatusCode;
 
        // set a default for logging exceptions
        bool bLogException = true;
        if (null == LogException)
        {
            // use the default for he ExceptionName to decide
            switch (ExceptionName)
            {
                case ExceptionName.NotOwnWorkload:
                    bLogException = true;
                    break;
                case ExceptionName.NotReportViewerForGroup:
                    bLogException = false;
                    break;
                case ExceptionName.WorkloadNotRecorded:
                    bLogException = false;
                    break;
                default:
                    bLogException = true;
                    break;
            }
        }
        else
        {
            // LogException not null so convert to Boolean
            bLogException = Convert.ToBoolean(LogException);
        }
 
        if (bLogException)
        {
            Elmah.ErrorSignal.FromCurrentContext().Raise(new Exception(ExceptionName.ToString()));
        }
 
        return "Exceptions/" + ExceptionName.ToString();
    }
}
```
Then, in this case, if workload isn't to be recorded, the method can return a view:

return View(ExceptionHelper.GetViewName(ExceptionHelper.ExceptionName.WorkloadNotRecorded));

**Note**: there is now an updated version of this code in [Updated error handling](https://mikebarram.wordpress.com/2015/02/10/updated-error-handling/)
