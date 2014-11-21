---
layout: post
title: Create a NFS instance on AWS
tagline: using Vagrant and Chef
categories: devops
tags: [nfs, vagrant, chef, aws]
---

I was creating AWS EC2 instances to install Oracle Fusion Middleware products, and I found
an stopper: How to download Oracle's installers? This could consume a lot of network bandwith
and I want to make this process repeatable, so I don't want to wait 1 hour each installation.

So I found this solution: [How to setup an Amazon AWS EC2 NFS Share](https://theredblacktree.wordpress.com/2013/05/23/how-to-setup-a-amazon-aws-ec2-nfs-share/)
But to make it reusable I create a Vagrant & Chef configuration to replicate and share this method
here:
