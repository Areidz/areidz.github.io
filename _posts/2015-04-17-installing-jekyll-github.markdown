---
layout: post
title: My first experience with Jekyll
date: 2015-04-17 17:34:16 +0200
description: How I installed Jekyll on GitHub Pages and my first impressions
img: clean-blog.jpg # Add Image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Jekyll, Template, GitHub]
---

After almost seven years using [Wordpress][wordpress-url] and [Blogger][blogger-url] as my main blogging services, I have decided to change my mind, make a step forward and install a simple web/blog with a great frontend and without a complex database and their vulnerabilities. Furthermore, I do not like the feeling of Wordpress owning the content of my blog because it is hosted there.

Having a look at the possibilities I decided to try **[Jekyll][jekyll-url]** on **[GitHub Pages][github-pages-url]**. Jekyll is a simple web/blog engine written in [Ruby][ruby-url] using static pages as entries and posts, so... no more databases!

Posts are written in **[Markdown][markdown-url]** style as raw-text and are automatically converted to static pages thought a template you can edit yourself.

## Installing the blog

I am using Windows as my main Operative System and Debian as my secondary one. Due to this, I decided to install the server on Windows. This installation and configuration was not a trivial step, so I followed the [official docs][official-docs-url] to do so.

The only problem I faced was installing *WDM*, which was not compiling in my machine. Nevertheless, everything seems to be working perfectly without it, so I am not going to try to fix it for a while.

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

## (July 2018 Update)

I have recovered some of the entries of my old Jekyll diary and I am posting them here, even though this blog has another template and design. 

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
[disqus-url]: https://help.disqus.com/installation/jekyll-installation-instructions
[share-url]: http://codingtips.kanishkkunal.in/share-buttons-jekyll/