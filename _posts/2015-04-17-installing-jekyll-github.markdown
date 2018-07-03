---
layout: post
title: Installing Jekyll with a custom template on GitHub Pages
date: 2015-04-17 17:34:16 +0200
description: How I installed Jekyll on GitHub Pages and my impressions
img: clean-blog.jpg # Add Image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Jekyll, Template, GitHub]
---

After almost seven years using [Wordpress][wordpress-url] and [Blogger][blogger-url] as my main blogging services, I have decided to change my mind, make a step forward and install a simple web/blog with a great frontend and without a complex database that could lead me to big vulnerabilities.

This is why I have decided to try **[Jekyll][jekyll-url]** on **[GitHub Pages][github-pages-url]**. Jekyll is a simple web/blog engine written in [Ruby][ruby-url] using static pages as entries and posts.

Posts are written in **[Markdown][markdown-url]** style as raw-text, and are automatically converted to static pages thought a template you can edit.

## Installing the blog

I am using Windows as my main Operative System and Debian as my secundary one. Due to this, I have decided to install the server on Windows. This configuration is not a trivial step, so I followed the [official docs][official-docs-url] to do so.

The only problem I had faced is installing *wdm*, which is not compiling in my machine. Nevertheless, everything seems to be working perfectly without it, so I am not going to try to fix it for a while.

## Folking the template

After looking for any good template to start the blog, I found **[Clean Blog][clean-url]**, an amazing template by *[Start Bootstrap][start-url]*.

I modified it to add support for *Disqus* following [this tutorial][disqus-url]. Thanks to this I have comments at the bottom of every post.

In addition, I have added share buttons following [this guide][share-url]. I had to adapt it to my custom template by creating some new css and html files, loading the css file in *head.html* and adding the html to the post template. Maybe you could find it interesting.

## Useful links

To finish the post, I want to share some useful links:


* **[Examples][examples-url]**: some examples of websites using *Jekyll.
* **[Jekyll][jekyll-url]**: main *Jekyll* website with install guides and configuration tutorials.
* **[Jekyll for Windows][official-docs-url]**: a website explaining how to install *Jekyll* on *Windows*
* **[Markdown Cheatsheet][markdown-cheatsheet-url]**: useful cheatsheet to write posts.


[wordpress-url]: https://www.wordpress.com/
[blogger-url]: https://www.blogger.com/
[jekyll-url]: http://jekyllrb.com/
[github-pages-url]: https://pages.github.com/
[ruby-url]: https://www.ruby-lang.org
[markdown-url]: http://daringfireball.net/projects/markdown/
[official-docs-url]: http://jekyll-windows.juthilo.com/
[clean-url]: http://startbootstrap.com/template-overviews/clean-blog/
[start-url]: http://startbootstrap.com/
[examples-url]: https://github.com/jekyll/jekyll/wiki/Sites
[markdown-cheatsheet-url]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[disqus-url]: https://help.disqus.com/customer/portal/articles/472138-jekyll-installation-instructions
[share-url]: http://codingtips.kanishkkunal.in/share-buttons-jekyll/