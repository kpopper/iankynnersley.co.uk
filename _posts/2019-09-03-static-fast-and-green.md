---
layout: post
title: 'Static, Fast and Green!'
date: 2019-09-03T16:24:45.075Z
---
Static websites are all the rage at the moment, and rightly so. There are a growing number of static site generators and some acceptable content management systems that broaden the appeal of static websites well beyond their initial developer user base.

Static sites can be hosted _very_ cheaply (often for free), require no high-spec servers and can even be served from basic [web-enabled file storage services](https://aws.amazon.com/s3/). 

They are also incredibly fast. With no database connections and no servers generating HTML they load many times faster than dynamically-generated websites a server can respond immediately. Even better, entire pages can be cached and delivered from CDN servers across the globe an order of magnitude faster again.

All of this has a massive but largely un-celebrated side effect: static websites consume **vastly less energy** than other websites. This is great news for helping address the climate emergency but can we go a step further?

I've been exploring ways to host static sites (like this one) on 100% green servers and have settled on a setup I'm fairly happy with.

### AWS S3
The _static web hosting_ option on an S3 bucket allows you to turn a directory of files into a static website. A site built with any static site generator (SSG) can be uploaded to an S3 bucket and hosted for a handful of cents a year. 

While Amazon has some distance to go on its sustainability journey, it does power a subset of its data centres with renewable energy and users can choose to use these by selecting [an appropriate region](https://aws.amazon.com/about-aws/sustainability/#AWS_purchases_and_retires_environmental_attributes,_like_Renewable_Energy_Credits_and_Guarantees_of_Origin,_to_cover_the_non-renewable_energy_we_use_in_these_regions.) when setting up their buckets.

To make hosting on S3 a bit simpler, it is possible to set up a [CodePipeline](https://aws.amazon.com/codepipeline/) that will automatically deploy updates from Github to your S3 bucket every time you make a change.

### Cloudflare CDN
Cloudflare is a powerful tool that makes it easy to manage domain names and SSL certificates. It also has an amazing trick up its sleeve: any traffic routed through them is cached through their CDN. This means that for free (on small websites) and with no setup, entire static websites can be cached across Cloudflare's global network of CDN servers.

Excitingly, Cloudflare have announced that [all their servers are now powered with renewable energy](https://blog.cloudflare.com/the-climate-and-cloudflare/)! 

### Conclusion
This combination of S3 and Cloudflare can give you a fully green hosted website that loads at lightning speed anywhere in the world. It is also optimised to minimise the energy used to build and transfer the website every time it's viewed.

If you want to suggest an improvement to this setup, feel free to [get in touch](mailto:hello+green@iankynnersley.co.uk).
