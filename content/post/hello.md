---
title: "100 Days of Code/Commitment Issues"
date: 2018-11-02T20:16:52-04:00
draft: true
---
Listened to [The Airflow Podcast](https://soundcloud.com/the-airflow-podcast), and two from Coding Blocks: [Docker for Developers](https://www.codingblocks.net/podcast/docker-for-developers/) and [How to Learn Programming Skills](https://www.codingblocks.net/podcast/how-to-learn-programming-skills/) today. From the latter I learned about the 100 days of code fad, and so here I am, hoping that maybe gamifying the process might get me to finally commit to writing a semi-consistent blog. Not sure yet how to, or even if I ought to, constrain the content, but whatever it is I'm just shooting to have enough content to make a couple bucks off some unscrupulous ad exchange suppliers (for research purposes).

# Day 1
Well I suppose getting this thing set up counts a little. And I can finally put my domain to use other than sitting around with one of my failed attempts at giving a shit about front end development.

Idk if I'm allowed to count work related things. On one hand I can't (for the most part) make the commits public. On the other hand is it work related if it never gets implemented?

## Airfleh
Yesterday I once again tried to tackle the soupy jenga tower of my organization's BI infrastructure with soapboxing about Docker and how there are ways to run an ETL pipeline other than printing out than printing out your code and faxing it to an AWS data center. Then I got very confused and then sad that I had wasted so much time (on something that nobody was really asking for anyway) and hadn't even progressed slightly towards the goal.

In keeping with tradition, after a failed attempt to re-architect the ETL pipeline, I woke up today with renewed enthusiasm and decided to (once again) deploy a proof of concept of [Docker Airflow](https://github.com/puckel/docker-airflow) using Cloudformation, EC2 and EFS. I'd really like to set up [Kube Airflow](https://github.com/mumoshu/kube-airflow) but I'm just not as familiar with Kube as I'd like to be and my recent battle with our cluster while trying to deploy [Jupyterhub](https://github.com/jupyterhub/zero-to-jupyterhub-k8s) has put me off for a while.

Anyway, I provisioned a new EC2 instance into our VPC, pulled the `docker-airflow` image and set up port forwarding to see the Airflow webserver from my localhost. So nothing *really* accomplished but certainly enough to merit a rum a coke.

## Oh yeah and this site
My annual search for "static blog generators" this year led me to [Hugo](https://gohugo.io/) which was simple enough to get started with, though at the time of writing I have not deployed it anywhere. So this may turn out to live in my ~/bullshit/ directory until next spring cleaning and just be another lesson in why you should do a bare bones tracer bullet before you do any feature development. Otherwise this should be deployed to [Netlify](https://www.netlify.com/) in about 10 minutes.
