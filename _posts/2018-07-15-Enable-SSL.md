---
layout: post
title: How to enable SSL for your custom domain name
excerpt: Suppose you came from the GitHub education pack and want a personal website using Jekyll and GitHub pages.
---

Suppose you came from the GitHub education pack and want a personal website using Jekyll and GitHub pages.
The following assumes you have already forked the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub and picked your custom domain name from namecheap.

Log in to namecheap -> Domain List -> Click Manage next to your domain -> Click Advanced DNS

Under Host Records, use ADD NEW RECORD to add five records: the four A records listed [here](https://help.github.com/articles/setting-up-an-apex-domain/#configuring-a-records-with-your-dns-provider) and one CNAME record pointing www to your custom domain name.

Should look like this:

![_config.yml]({{ site.baseurl }}/images/nc_records.png)

Add your custom domain name (without the www) to your CNAME file in your forked repository.

Click Settings page for your forked repository and check "Force HTTPS" when it becomes available.
