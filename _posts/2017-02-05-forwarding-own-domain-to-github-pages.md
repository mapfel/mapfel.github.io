---
layout: post
category : lessons
tagline: "Supporting tagline"
tags : [github-pages, godaddy, tutorial]
---

# Overview

That blog post explains the intention of using Github Pages to host own blog content. It describes also how to configure a new [GoDaddy](www.godaddy.com) domain to have a nice entry point into this blog.

## Motivation

Over several years I've blogged via [Geeks With Blogs](http://geekswithblogs.net/mapfel/). But as more I've maintained an internal wiki of my development team, it felt wrong to write content with an WYSIWYG editor. I came in love with Markdown and Git-based repositories.

Additionally the question came up: "Why writing for another provider instead of myself?"

Therefore it was clear that it is necessary to move my blog away and switch to a toolchain with Markdown and Git.

# Realization

## Github Pages

### Overview

Initially the blog should be hosted on one of my existing domains with vServer infrastructure in the background.

But that step was to big because of some additionally familiarization with Git on the hosting site.

That will be investigated somewhere in the future.

So for the first phase it is good enough to use Github Pages to host my static content.

### Prepare the blog

To use Github Pages as a provider for own blog content it is necessary to create a Git repository for it. Yes, only a Git repository holding the blog content as static web sites is necessary to serve the content.

Create a new repository and name it <your-user-name>.github.io. That's all. Now you have a base to start.

Check the state of your Github page in a browser with ```http://<your-user-name>.github.com```.

## GoDaddy

In the meantime a new domain [apfel.space](www.apfel.space) is used as an entry point to my hosted content. A *.space domain is very cheap - only $15 for two years. So it's a good deal, pay some bucks and avoid side effects for existing stuff.

### Configure new domain

After ordering the new domain you have to configure a forwarding to your Github page from your new domain.

Unfortunatelly I was not able to switch the UI language to English. So the screenshots have German texts. (a ticket was created to GoDaddy).

1. Select the domain to configure  
![Use my domain]({{ site.url }}/images/20170205.GoDaddy.01.small.png)

2. Connect it with an already existing web site (your Github Page)  
![Connect]({{ site.url }}/images/20170205.GoDaddy.02.small.png)

3. Configure the ```A``` entry to point to the IP address of your Github Page and the CNAME for ```www``` to point to the address of your Github page.  
![Configure entries]({{ site.url }}/images/20170205.GoDaddy.03.small.png)

4. Wait a while (till 1h) to get the update populated
