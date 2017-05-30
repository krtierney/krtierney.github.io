---
layout: post
title:  "Switching to Netlify"
date:   2017-05-30
permalink: /2017/05/30/switching-to-netlify/
---

This site had been using GitHub Pages for hosting for the past N months. I use
Heroku for most of my projects, so paying for a hosting service just
for this simple static site felt like a waste of money. Plus, I wanted to
give GitHub Pages a go and see how it all worked. It was fine, mostly, except
for one massive, glaring issue: If you use a custom domain with GitHub Pages, 
it's really not a simple matter to add an SSL certificate
and force connection over HTTPS. This has been low-key irritating me for ages,
but all of the
[solutions](https://hackernoon.com/set-up-ssl-on-github-pages-with-custom-domains-for-free-a576bdf51bc)
I've found require you to use Cloudflare as a CDN, and
I'm trying to
[avoid](https://www.propublica.org/article/how-cloudflare-helps-serve-up-hate-on-the-web) 
relying too heavily on their services.

Anyway, wow, [Netlify](https://www.netlify.com)! It's amazing. It took me less
than five minutes to create
an account, trigger a build from my [master branch on
GitHub](https://github.com/krtierney/krtierney.com)
and verify that
everything worked well before moving my DNS over and adding an SSL certificate.
I couldn't be more impressed. The only final step was renaming my repo on GitHub
to disable the link with GitHub Pages. Response times for loading the site have
also been slashed by about 80%. If I'd known it would be this easy, I would have
done this months ago. It's so simple I'm tempted to build fun little sites for
every random domain I have registered, just to see how fast and easy the setup
is with Netlify. So far, I'm an extremely happy customer.
