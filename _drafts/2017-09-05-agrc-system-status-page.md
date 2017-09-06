---
layout: post
status: publish
published: true
title: 'AGRC System Status Page'
author:
  display_name: Steve Gourley
  email: sgourley@utah.gov
date: 2017-09-05 18:29:31
categories:
  - Featured
  - Developer
tags:
  - monitoring
---

Over the years, GIS is trending more and more towards being web-based. AGRC has tried to keep step with this trend with the addition of the [discover server]({{ "/discover" | prepend: site.baseurl }}), mapserv and its over fifty map data services, the TurnGPS RTK GPS service, and the [Web API](https://api.mapserv.utah.gov) handling over one million requests per month. More and more users are relying on these services. Outage are _very_ disruptive and users want to know what is going on and when AGRC will resolve the issue.

AGRC is now maintaining a system status website for the services we provide. Users can visit and bookmark https://agrc-status.netlify.com to check on the status of AGRC systems. 

If you notice an outage, please check the [website](https://agrc-status.netlify.com) **first** as this will get you the details quickly and it leaves us with more time to work toward resolution. If you do not see the status accurately reflected on the status page, please get in contact with us immediately by [phone or email](https://gis.utah.gov/about/contact) with a description of the problem.

When outages occur, AGRC will use the status website to let users know that:

1. We are aware of the issue
1. The suspected cause of the issue, and
1. When will this be working again?

We will continue to use [twitter](https://twitter.com/MapUtah) with the hash tag [#utmap](https://twitter.com/hashtag/utmap) to disseminate information about outages and other interesting news. But, AGRC recognizes twitter _does not_ reach all our users and that email is private. Not every GIS user has a twitter account and not every person with a twitter account follows us or comprehensively reads our tweets.

Lastly, if there is other systems that you would like us to track, let us know.

## Technical Information

As you may know, the fine people at Netlify host gis.utah.gov. They offer a great service and when they released [StatusKit](https://www.netlify.com/status-pages/), AGRC was very excited. StatusKit is a website and template for [Hugo](http://gohugo.io/).  Hugo is a static website generator, similiar to [jekyll](https://jekyllrb.com/) which generates this website, built with [Go](https://golang.org/). Using pull requests or a desktop CLI tool, we can create new incidents and Hugo and Netlify take care of the rest.