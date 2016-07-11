+++
date = "2016-07-07T11:43:36-06:00"
draft = true
title = "Deploy a Static Blog in 7 minutes."

+++

I learned that Caddy+Hugo is a very slick combination. John recommends Wordpress for setting up your blog because it is easy: you can do it in 5 minutes.  I want to see if I can match that with Hugo+Caddy.

Here is the plan:

 * create a docker container with caddy+hugo installed
 * create a form to build a config file
 * create a script to deploy to an Amazon EC2 or a Digital Ocean droplet.
 * have user run the script
 * assume that the domain is already registered
 * provide instructions to point the domain name to the running instance
   (investigate Gandi.net APIs to do this from the script.)


 Future: Do the same for a mail toaster. Sell in AMI marketplace?
 
