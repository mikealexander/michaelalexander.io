---
layout: post
title:  "Hello, world!"
date:   2015-05-10 16:30:51
categories: news  	
---
I've just set myself up with my new website and blog.  I wanted somewhere to note down my technical problems and how I (attempt to) 
solve them, as well as my thoughts on the tech world, startups and life.


Jekyll
-------
I build the website using [Jekyll: the blog-aware static website generator][jekyll].  It's really an amazing tool.  Basically, you define your
posts in [Markdown][markdown] (or you can write a converter for any markup you prefer), and Jekyll churns out your whole blog/website 
as static html files which you deploy to you server.  No databases, or expensive server-side processing, just super fast static files.
It makes use of the [Liquid templating system][liquid], allowing you to split your website into re-usable components, implement pagination,
use conditional logic and more.

[jekyll]:      http://jekyllrb.com
[markdown]: http://en.wikipedia.org/wiki/Markdown
[liquid]: http://liquidmarkup.org/
