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

But to make it more reusable, I create a Vagrant & Chef configuration to replicate and share this method
here: [NFS-Server branch](https://github.com/jeqo/vagrant-aws-chef-nfs/tree/nfs-server)

## What are the steps?

0. You need to install Vagrant (vagrant-aws and vagrant-omnibus) and Chef SDK
1. You have to create Chef Server account
2. You have to create a Vagrant configuration
3. Test it.

Well, I create a configuration on GitHub and I'll show you how to use it:
