+++
date = "2016-07-05T10:09:15-06:00"
draft = false
title = "Lernisto.com is Live"

+++

I have a accomplished the first AWS task: lernisto.com is live on Amazon S3.

Let me remember the steps:

 1. create an AWS account.
 1. follow the walkthrough [Example: Setting Up a Static Website Using a Custom Domain](https://docs.aws.amazon.com/AmazonS3/latest/dev/website-hosting-custom-domain-walkthrough.html)
 1. register a domain name.
 1. set up Route53 to point to the bucket.
 1. set the domain to use Amazon's Route53 name servers.
It seems necessary to use Route53 because you cannot have a CNAME for a root domain. Route53 works around this with code that fakes an A record with an internal CNAME pointing to the bucket endpoint. Amazon probably knows more about running nameservers than Godaddy anyway.
 1. I ignored the instructions to manually create the index.html and error.html, because I know that is not the right approach.
 1. Instead, I had to
   1. install the AWS command line client: `pip install awscli`
   1. configure it use my credentials `aws configure`
   1. build the web site `hugo -t lernisto-zen`
   1. upload it: `aws s3 sync public s3://lernisto.com`
