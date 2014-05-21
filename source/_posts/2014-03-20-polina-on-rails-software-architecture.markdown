---
layout: post
title: "software architecture primer"
date: 2014-03-20 22:45:56 -0400
comments: true
categories: 
---

Software Architecture

Stack Overflow architectures:
http://www.dev-metal.com/architecture-stackoverflow/


Three main concepts:

     Stakeholders

     Viewpoints

     Perspectives

Sketch functional structure of system
     Start grouping components into processes- where processes will run in data center
     Operations group-- system management components
     Data-- adds main data stores and annotates data flows between key components

     Problems:
          The developers are distracted by operational components; servers, disk arrays
          Worry about the way the app will be deployed to data center
          IT people like the system management software but keep asking questions about the data flows


Consider the system's architecture through a number of distinct views
     Communicate a system in a partitioned fashion
     ex Functional Structure, Information organization, Deployment environment
     Still problem: which views to use and how to create each one
          Solution: use template views (architectural viewpoints)
                    Guide to process of developing views that describe architecture

Two main questions to answer;
1. what a system does?
2. How does it provide its services
     How quickly it runs, how secure it is, how available it is, how easy is it to modify, many different nonfunctional factors--> quality properties

Quality properties--> cross-cutting concerns

Achieving your quality goals affects all of your different template views

Architectural viewpoint-- addresses the needs and views of stakeholders
Architectural perspective-- addresses performance, security, availability