---
title: Glasgow University Tech Society Website (From Django to Jekyll)
updated: 2016-10-17 17:32
type: project
---

![GU Tech Soc Website](/assets/techsoc-website/techsoc.png)

> You can view the live website at [gutechsoc.com](http://gutechsoc.com)

The Glasgow University Tech Society's goal is to bring students closer to the tecnology and topics that interest them.

I originally created the techsoc website on AWS using Django - we'd log in to the admin panel about 3 times a year to add some new information to our database and Voila! It would be rendered in to HTML every time a user visited the page.

This was all well and good, but we were really only using it to serve the same static webpages to every visitor, so generating it every time was incredibly wasteful. When we found out we were running up a £20+ AWS bill every month we had to look for a better solution.

### Enter Jekyll on Github Pages

For this we used Jekyll on Github pages, which is a fantastic alternative to running a fully blown framework when all you want to do is serve some static webpages. You still get to render data in to the pages programmatically using the Liquid templating language, but the key factor is that this is only done once every time you change your data or layout. Github also provides free hosting on [github.io](https://github.io).

All that was left to do after I had translated the Django templates to Liquid (and the SQL database to YAML) was to hook up our GoDaddy domain using [this guide](http://andrewsturges.com/blog/jekyll/tutorial/2014/11/06/github-and-godaddy.html) by Andrew Sturges.

> The github repo for the techsoc website can be found [**here**](https://github.com/gutechsoc/gutechsoc.github.io).
