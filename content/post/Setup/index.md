---
authors:
  - admin
categories:
  - Academic
date: '2019-03-24T14:09:48.000-04:00'
featured: false
subtitle: Why and how
summary: This is an introductory post of why and how I set up my personal website
tags:
  - website
  - programming
  - coding
title: Setting up a personal website
image:
  caption: 
  focal_point: 

---
## Motivation

I finally decided to build and maintain my personal website after contemplating on multiple factors. My biggest deciding factor was an outcome of my recently completed MBA - the question was : Whats my ROI (Return on Investment) of making a webpage in terms of time, money and effort. As you can tell, I decided to build the website because I found an easy to use, minimal time and effort based setup which was fairly inexpensive (even free if you would like). This post explores the setup and how I build it in hopes that it may help others to follow.

## The Setup

I explored numerous options like Wordpress and university page hosting using drupal/wordpress etc - I realized that dynamic hosting required too much maintenance and I was not ready to devote that much time. This lead me to the path of Static Site generators and although there are numerous options like Jekyll, Pelican etc and plenty of comparisons of pros and cons for each online, I settled on Hugo because of the following reasons:

* It has a great theme available for academics conveniently named Academic.
* It has a great community and is under active development with [George Cushen](https://georgecushen.com/) doing an amazing job devoting his time and actively listening to feedback and constantly making improvements.
* It is lightening fast and takes milliseconds to build the website.
* It can be hosted on netlify.com via github for automatic deployments.

### Installation and Customization

The setup was remarkably simple because the [Academic theme documentation](https://sourcethemes.com/academic/) is great and guides you through the entire [install](https://sourcethemes.com/academic/docs/install/) / update process. It literally took me 30 minutes to get the initial structure of the website setup. The level of [customization](https://sourcethemes.com/academic/docs/customization/) I could achieve was also extremely well documented. I tweaked it to my liking as far as color/fonts are concerned and settled on something that was simple and elegant. I also setup disqus comments and google analytics - all of which are covered in the documentation of the theme.

### Custom Domain

With the bulk of the hosting cost eliminated since the netlify /github combo is completely free, I decided to look into the possibility of registering a personal domain name. Namecheap.com offers great cheap hosting but after some research, I decided to go with NameSilo.com since they offer cheaper domain names with Whois privacy and no up-sell/marketing. I have not had any problems with them and it only cost me 5.99 USD for the first year with 8.99 USD renewal rates. A detailed comparison on this and other hosting solutions can be found on [this article](https://medium.com/@steelwagstaff/how-to-make-a-website-d1e83f30043b) which actually led me to NameSilo.

### CMS Options

I was satisfied with the setup but the last piece of the puzzle was easily posting stuff on the website. While writing in markdown locally using VS Code and committing to the github repository worked, a more streamlined solution would be great. This is when I discovered forestry.io. It works with Jekyll and Hugo both and has a great UI. Initially forestry.io was not working because it did not support subfolder config.toml architecture. Their support was awesome and suggested I add a blank config.toml file in the root, which fixed the problem [^1]. I got the inspiration from [this blog post](https://haodong.io/blogging-with-hugo-and-netlify-and-forestry-io/).

## Conclusions

All in all, I am very satisfied with my inexpensive, easy to use setup which establishes a clean, professional presence online. The setup is as follows for anyone wishing to host their own academic website:

1. Static site using [Academic](https://sourcethemes.com/academic/) theme on Hugo
2. Served using Netlify.com hosted on Github.com
3. Web domain registered through Namesilo.com
4. Blog posts using forestry.io

[^1]: This post is edited using forestry.io and seems to be working. One small gripe is that the preview system is very slow even for individual blog posts.