---
title: "Getting this site started"
date: 2020-04-09T22:02:26-04:00
draft: false
## Deploying Hugo with <ProductName />
---

So I've tried to start a few site in the past, they never turned out well, mostly because I gave up on them after two weeks.

But recently I started reading more and more blogs causing me to get another itch to try again. 
This time I decided to go with Zeit's Now service, there isn't much reasoning to this except that I wanted to try something new.

Now, the configuration of this workflow is really simple. All it really consists of would be GitHub and Now primarily, through in VSCode locally and Hugo and boom you're done.
So I don't really feel like a tutorial is really needed, instead, I think it would be beneficial to have more of a comparison discussion about other services that I've used.

# Netlify
When someone things of a fully featured front end hosting platform Netlify is easily one of the ones that most people would go to. It's free, integrates well with GitHub and overall had a great marketing strategy,
I've been hearing about them a lot in some development podcasts. I like Netlify they're easily one of the ones that I would send people directly if they were looking for this type of service. It's probably the complete package
when talking about a kitchen sink service.

The only downside that I've felt about Netlify was that it just felt a bit heavy, like it kinda tried a little too hard in order to suit everyone.
There's nothing wrong about this, don't worry, I just wanted something simpler, nothing too fancy.

Overall I would give Netlify an `A` for most people, if you cherish minimalism you can go ahead with Netlify but there are others out there that would probably suit your fancy.

# Amazon S3
Talk about simple as simple can get, I know plenty of people that Host their static websites on S3 just because that's all their site is, static content that doesn't change often. This is totally where Amazon S3 as a hosting
platform comes to shine. There's really nothing you have to do special here. It boils down to two steps:

1. Upload your site to your S3 bucket
2. Slap a CNAME record on your domain to you bucket

That's really it you have a fully functioning static website that can host your content. Perfectly for what true minimalists want.

# GitHub Pages
GitHub Pages is the cult classic, it's great for people who love GitHub and love git workflows. Similar to Amazon S3, it's perfect for those static websites that people love to host. But here you have one extra step,
but integrates nicely with people's development workflows.

Make your changes on any branch of your github project, when you're ready to push to master/production merge your changes into the `gh-pages` branch instead of some kind of itegration hooking into your repo and deploying your static weapon.
