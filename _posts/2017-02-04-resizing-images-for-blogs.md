---
layout: post
category : Tipps&Tricks
tagline: "Supporting tagline"
tags : [github-pages, godaddy, tutorial]
---

#Overview

Often enough the screenshots, supposed to use for blogging, are too large for the blog post. Especially by using a display with high resolution (Retina and Retina like displays) this affect almost each screenshot.

Such a large screenshot in a blog post looks not nice and often the right side is cropped.

This blog post describes my toolchain for resizing screenshots on Windows and macOS.

## Windows

### Make the screenshot

Usually I create my screenshots with [**Greenshot**](www.greenshot.org). It allows the user easily to add some symbols and text. Depending on the scaling later I ensure to have multiples of 2 or 4 as the size on both axes. (see below)

### Scale the screenshot

After saving the all the screenshot I resize them all together with [**Image Resizer for Windows**](http://www.bricelam.net/ImageResizer/). 

**Image Resizer** creates a new menu entry in the **File Explorer** which appears by right mouse clicking at a image file.

Depending on the original size I scale them down to 25 or 50 percent (not pixels). With these values I hope for a perfect quality. That's why I chose these multiples.

The tool saves the shrinked images with a new filename next to the existing files. The new name is the old name suffixed with ``` (Custom)```.  
e.g.  
```WindowsServer.IIS.Install.06.1.png```  
becomes
```WindowsServer.IIS.Install.06.1 (Custom).png```

### Rename the screenshot

Since years [Joe](https://tools-and-more.com/Central/Produkte/Software/Dateien_und_Dokumente/Joe/) is my friend for renaming. (btw: some older versions are still available and for free).

The renaming pattern ```[R10-].small.[typ]``` replaces the last 10 chars of the filename with the text ```.small```. So the sample above transforms from  
```WindowsServer.IIS.Install.06.1 (Custom).png```  
to  
```WindowsServer.IIS.Install.06.1.small.png```

![Joe in action]({{ site.url }}/images/20170204.Joe.1.png)

## macOS

t.b.c.

Starting points:

1. Make screenshot with CMD + CTRL + SHIFT + 4
2. Save it (paste it onto OneNote and save it from there)
3. Copy all screenshots
4. Preview all copied screenshots
5. Use the Adjust size function
6. Save all during quit
7. Rename the shrinked images with Finder
