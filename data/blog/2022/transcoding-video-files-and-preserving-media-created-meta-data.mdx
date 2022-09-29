---
title: "Transcoding video files and preserving \"Media created\" meta data"
date: "2022-09-08"
tags: ["windows"]
draft: false
---

VLC is a handy tool for transcoding video files - in my case, mostly from .MOV to .mp4

- From the Media menu, select "Convert/Save…"
- Add some files
- Click "Convert/Save" button
- Choose a conversion profile or click the spanner icon to create your own, combining your preferences in video and audio codecs
- Choose a destination file (unless multiple files are being converted)
- Click "Start"
- Wait a while and hopefully all of your videos will have been transcoded

Then you find that you've lost the "Media created" meta data for transcoded files has been set to the date/time of the transcoding, not the original date that the video was recorded, and that's the one that you want to sort media by.

Assuming you've not deleted the original files, you can get the meta data back in this convoluted way:

For all of the old files, write the meta data to a text file and then, for the newly converted files, update the meta data from the text file - as described here:  
[https://superuser.com/questions/482868/batch-converting-a-video-while-keeping-the-original-time-stamp-creation-date](https://superuser.com/questions/482868/batch-converting-a-video-while-keeping-the-original-time-stamp-creation-date)

This only allows certain properties to be updated, listed here:  
[https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about\_properties?view=powershell-7.2](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_properties?view=powershell-7.2)

This doesn't include the "Media created" property, so instead update CreationTimeUtc

Then install [Exiftool](https://exiftool.org)

At the command line, you can get a list of the time properties available in a file:  
```c:\\some folder\\"exiftool(-k).exe" -G1 -a -s -time:all d:\\Videos\\probably\_kids\_messing\_about.mp4```

Then, you can update the meta data for all of the files in a folder like this:  
```c:\\some folder\\"exiftool(-k).exe" -api QuickTimeUTC "-CreateDate<FileCreateDate" d:\\videos\\mp4\\```

The CreateDate property is updated with the value of the FileCreateProperty

Next time, I'll use [Handbrake](https://handbrake.fr/), which I believe has an option to preserve meta data when transcoding...
