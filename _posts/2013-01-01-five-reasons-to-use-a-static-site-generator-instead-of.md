---
layout: post
title: Blogging like a hacker
excerpt: Back in 2000, when I thought I was going to be a professional writer, I spent hours a day on LiveJournal doing writing practice with other aspiring poets and authors. Since then I’ve blogged at three different domains about web standards, print design, photography, Flash, illustration, information architecture, ColdFusion, package management, PHP, CSS, advertising, Ruby, Rails, and Erlang...
description: A new year approaches and one of my New Year's resolutions is to hack more. I began by creating a personal Jekyll blog. Little did I know that it was going to be so fun.
category: blog
---

> source: <http://blog.guestlistapp.com/post/2304152860/five-reasons-to-use-a-static-site-generator-instead-of>

When we sat down to build the Guestlist website, we thought we’d try using Jekyll, a “blog aware” static site generator written in Ruby. The basic idea is that your website is composed of a number of layouts, pages, and blog posts, which Jekyll stitches together into a set of static files during a single build step – not at runtime. This gives us a couple of neat advantages over traditional hosted publishing software like Wordpress, which generates pages dynamically.

Static files are fast

With Jekyll, you are serving your website content directly from the file system, instead of handing off to a dynamic process (in Wordpress’ case, PHP). Serving static files is fast – as fast as it gets. This means we don’t have to worry about being Techcrunched or getting hammered with traffic because our web server can stand up to it.

Source control friendly

Instead of managing all your content inside Wordpress’s database, it’s being managed via source control – in our case, Git. That means we can work on the website when we’re offline, seamlessly share changes, and browse history online via GitHub. And since Git repositories are distributed, backing up our data isn’t a concern.

Less security concerns

Since Wordpress is hosted software operated over the web, it means dozens of potential injection vectors are publicly accessible to would-be attackers. And as you’re probably aware, vulnerabilities have been discovered. Contrast this with Jekyll, which does all its work offline and off the server; it’s a tougher nut to crack.

Easy to deploy

Unlike Wordpress, I don’t need to install Jekyll on a single server – just my local development machine. Our deploy process is to build the site locally, then rsync the result to a remote server. The whole process takes seconds. Compare this to having to manage multiple Wordpress installs on multiple servers, keeping them all up to date, backed up, and humming smoothly. That’s a lot of maintenance.

Use your favourite editor

I don’t know about you, but editing blog posts in a 300 x 300 textarea isn’t my idea of fun. With Jekyll, I can fire up TextMate and write away, complete with spell checker, Textile syntax highlighting, and other useful goodies. Using the same editor to write blog posts as I write code also gives me a warm, fuzzy feeling - for whatever that’s worth.

So, those are some compelling reasons to use Jekyll. There are downsides, of course – what happens when you want to insert dynamic content, for starters? But that’s an article for another day.