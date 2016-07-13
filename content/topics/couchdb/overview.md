+++
date = "2016-07-13T14:11:43-06:00"
draft = true
title = "CouchDB Overview"

+++

## What is it?

CouchDB is a [document-oriented data store focused on the AP](http://blog.nahurst.com/visual-guide-to-nosql-systems) of the [CAP triangle](https://en.wikipedia.org/wiki/CAP_theorem). The data store sacrifices strong consistency in order to provide availability in the face of a network partition. The system uses MVCC to provide eventually consistency. The documents are JSON objects. Queries are supported by Javascript-based map and reduce operations.

## Why do I want to learn it?

I am evaluating CouchDB as a candidate data store for a password manager to replace LastPass. (It bothers me that LastPass is not free software, and I don't like that the developers seem focused on adding new eye-candy features that make it slower. As a critical part of my trusted computing base, I want my password vault to be simple and rock-solid.)
It might also work well as a store for a chat app to replace WhatsApp/Messenger/SMS/MMS. I don't want to spend more money than necessary on airtime for my cell phone.
My first project ("something useful") will be a dream-catcher.
