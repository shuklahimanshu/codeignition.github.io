---
layout: post
title: "How to Create a Low Cost, Self-Healing & Immutable Infrastructure using AWS EC2 Spot Instances [Part 1]"
description: "Reduce AWS bills significantly & automate maintenance using Auto-Scaling"
tags: ['aws','ec2','spot','infrastructure','cloud','devops']
author: vipul
---
{% include JB/setup %}
If you have ever used any cloud service, then chances are pretty good that it was AWS. They lead the way with almost 1/3rd of the cloud infrastructure market ([source]("http://www.cloudcomputing-news.net/news/2015/feb/03/aws-hits-five-year-high-cloud-infrastructure-market-share/" target="_blank")). Worldwide more and more professionals are using AWS’s EC2 instances because they are dependable, flexible & easy to manage.

But all that comes at a cost, which companies realize soon enough. Because when you grow, your EC2 bill grows with you. I had already heard stories of large bills before experiencing this myself. And when it happened to me, it made me stop and ask some questions.

What are your options when the AWS EC2 bills start growing too much, too fast? Do you: 
a.	Move to another cloud service?
a.	Move to DataCenters? 
a.	Raise the money to pay the bills anyway?

Or do you find a way that both saves money & makes managing it easy? By introducing Spot Instances into the mix and deploying Auto-Scaling, you can do just that.

**Spot Instances**

To the uninitiated, Spots Instances are the unused or dormant compute resources which AWS provides to bidders at much lower prices than normal instances. On an average these prices can be 1/8th or 1/10th of normal instances, and the variation is totally dependent on market demand where AWS users place bids.

It works like any other auction market, in that AWS sets a base price and users put forth bids at prices higher that the base price. The highest bidders win & it’s smooth sailing after that.

Except it isn’t, because Spot Instances are temporary allocations of unused resources. Spots are yours so as long as someone else doesn’t bid a higher price for them or there isn’t increase in demand for normal instances. These are the termination policies exercised by AWS, and they are the reason why a lot of people don’t opt for Spot Instances in their mix. 

*Continued in part 2*