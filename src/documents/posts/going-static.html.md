```
title: Static Site Generation with Docpad
layout: post
tags: ['intro','post']
intro: Going static seems to be all the rage now, with tools like Docpad, Jeckyll, and Octopress. I started doing web development in 1995 and of course at that time, all websites were just a handful of html pages and images uploaded to your live server via FTP. Our sites were already static.
```

Going static seems to be all the rage now, with tools like [Docpad](http://docpad.org/), [Jekyll](http://jekyllrb.com/), and [Octopress](http://octopress.org/) (based on Jekyll). I started doing web development in 1995 and of course at that time, all websites were just a handful of html pages and images uploaded to your live server via FTP. Our sites were already static.

<blockquote class="content-quote">
	Automation doesn’t come without a cost - or a sense of irony.
</blockquote>

Granted, our website objectives were very simple back then. As things became more complex, organizations realized that static sites were just not scalable. Web servers were put to the task of automating a lot of the work that we did manually. This relieved a lot of the burden, but because of this, we were put into a new role. Instead of coding HTML for every page we were now teaching computers how to do it for us with scripting languages like Perl and PHP. Even without the use of databases, think about how much more complex a website is simply by adding PHP. Then throw in a content management system backed by a mysql database and what was once a job that could be done by a single html developer now has to be done by a designer, a php developer, a database administrator, and systems engineer. Automation doesn’t come without a cost - or a sense of irony. Automation requires scaffolding, and scaffolding needs to be maintained and improved. 

As websites and web applications become more complex connecting to different services and databases, you begin to realize that actually the overwhelmingly vast majority of websites including blogs are really not all that complex relatively speaking. However, if I as a team of one developer working for myself, want to write a blog, there are a lot of considerations I now must think and worry about. How quickly can I learn how to build a theme? Is my site and database secure? How often do I need to update my software? Is my site going to load fast? Can my site handle large and sudden spikes in traffic? What about data recovery? For the average developer this can become overwhelming.

So why are things so complex? The reason is because we love to automate. We’ve grown accustomed to a narrow definition of automation though. We tend to think of automation happening on the server and in real time. So from that perspective the only way to automate is to install software and a database on our web servers and let the web server generate the site for us. As mentioned, this is not without a cost. For most developers, this cost is becoming too high.

This is why static site generation is becoming more popular, at least within the developer community. We’re starting to ask questions like why does this automation have to happen on the server? Also, we’ve been caching our sites! What else is caching but a form of static site generation? If that’s the case, why can’t I just have all that work happen on my own computer then just push the “cache” to my server when I want to deploy? As a web developer I have a whole bunch of tools on my computer that help me automate all kinds of stuff now, why not site generation?

This is what Docpad lets me do. With it I can work completely local and without a database. I can create a new blog post just by creating a new html file, add some meta information to it such as title, what layout template to use, and just start typing my post. As I save the file, docpad watches for changes then generates all the necessary html for me. All my pages and posts, css, and images, get saved to an output folder, which can then be uploaded to any web server and served 100% statically.

All the complexity is hidden on my own machine and not on the server where those complexities can potentially be exploited. Yet the biggest advantage for me is that I now have a single source of truth for my entire website. All my code, and all my posts can go into a single version control system (like git). Potentially, if I wanted to create a new blog post and keep it as a draft, all I have to do is create a separate "draft" branch for it. Then When I'm ready to publish I can merge it into the main trunk.