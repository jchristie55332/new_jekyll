---
layout: post
title:  "First steps into Ops"
date:   2016-04-09 21:44:00
categories: development tools
---
So recently I've been taking a strong interest in the world of Web Operations.  I think its an important skill for every developer to understand how deployment works and fix and troubleshoot any issues that may arise.  I am by no means an expert in the world of severs and deployment but I have learnt a lot recently and intend to continue to do so.

At Third Space Learning we use Amazon AWS s3 to host all of our services and Capistrano for all deployment scripts.  I have experience using the Heroku tool belt which is an absolutely fantastic tool, however extremely expensive and I really don't understand how companies are going to market using it.  Capistrano functions in a very similar manner to the Heroku tool belt does once you have it up and running, its the getting it up and running thats the issue.  There are certain configurations that Capistrano assumes and being very inexperienced I tried and failed to fight against them. Please do not.

On the server I have only experienced using Nginx. Usually I would try something else but it is such a good tool that I have no urge to try anything else.  It allows you to forward traffic as you wish to multiple apps, serve static content and manage permissions with relative ease.  To run Nginx I tend to include an nginx.conf file that handles the domain being used and the linked .sock file that handles the routing.

I only have experience using Capistrano with Node and Ruby applications.  For Node applications I find it an impure method of deployment as you need a knowledge of Ruby to deploy a Node application which seems very backwards, but I will move on.  To demonise a Node application I use pm2 as its supper simple to manage and very lightweight.  For Ruby applications I use Unicorn as it seems to perform the same function.  I generally link the deployment files for the demonise functionality into the Capistrano shared folders which allows them to be stopped and restarted very quickly during the deployment, which allows almost zero downtime.

I'm not going to go into the the actual files as its pretty dry to walk through but I think its a fantastic thing for a developer to look at as its such a large part of our job.  If anyone is interested in how I deploy apps or need any help I will more than happily go for a couple of beers and talk it through.  Otherwise have a great weekend.
