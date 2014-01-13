---
layout: post
title: "yet another static site generator"
description: "how to build your own static site generator"
category: cs
tags: [ruby, projects]
---
{% include JB/setup %}

There are lots of static site generators out there-- 212 of them in fact! See http://staticsitegenerators.net/.

Why go about building your own static site generator?

Well, there were a few things about static site generators that I found really handy:

You can create content in markdown/textile
You can manage everything with git
You can publish directly from the terminal
No database to maintain
No hosting headaches-- host on github
Makes your code completely open source-- yay!
They can turn your site into an open source project 
High performance: static HTML pages can be immediately served by web server because there is no database requests or other overhead. 
No special software needs to be installed, and the processing/memory requirements are low 
SSG allow you to follow whatever workflow you like
Any input format that can be transformed to HTML can be used
Use the version control system of your choice
The use of SSG makes the creation of your website into a process akin to software development-- any budding swe will think that's awesome


As a budding hacker, one way you can learn is by taking things apart and then putting them back together. That is what I will strive to do with Jekyll-Bootsrap.

Jekyll-Bootstrap is the static site generator that I am using to power this blog. It provides a full blog scaffold for Jekyll based blogs. That means I will have ot peer into Jekyll to see what's going on and see if I can recreate my own, customized version of a static site generator. 

Another reason I wanted to do this project was that I wanted to explore another way to build a website. There are many ways to go about building a website. You can write HTML manually, use a framework to create dynamic web sites (see my post on web frameworks), or use a full fledged content management system (CMS) that offers an interface to create, edit, review, and publish your content. The Wellesley College website currently uses Drupal as its CMS.

You can also use tools to generate static (instead of a dynamic) website. 

What the SSG will do:

Once you have written some input files and created a layout along with rules to specify how files should be compiled, the site generator will do the rest for you. The compiler will take every changed item and produce output by running your specified transformations on the input. It can also be configured to deploy the site for you (heroku, github pages, what have you). An SSG also allows you to run checks on your output-- it can validate the CSS, HTML, find stale files, and find broken links. You can add further checks with a few lines of code. 

Goal: the time of routinely writing HTML by hand is OVER. On to the static site generators! It's so much nicer to just write your content in Markdown and let the SSG do the rest for you.

This article still in progress.

Take a look at this for now: https://github.com/skx/static-site-generators




