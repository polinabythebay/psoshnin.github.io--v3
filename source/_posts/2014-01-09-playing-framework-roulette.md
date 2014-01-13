---
layout: post
title: "playing framework roulette"
description: ""
category: 
tags: []
---
{% include JB/setup %}

Client-side frameworks are the way to build rich web apps

### The lowdown on JavaScript Frameworks/Libraries:

What all of the frameworks agree on:

Serious JS apps require proper data models and ability to do client side rendering, not just server rendering + Ajax/jQuery code

All use the model-view-* separation. There’s some kind of controller piece, but it can depend on the framework.

Data binding = Good
All frameworks except Backbone and Spine have built in declarative data binding in their views

Every single framework is MIT licensed and hosted on GitHub

JS Library vs Framework
Library: can put in your existing architecture and add specific functionality
Framework: give you an architecture (a file structure) that you are meant to follow and are meant to handle common requirements

Libraries don’t make your architecture so deeply tied to the project — they’re typically easier to learn, adopt, customize, and minimize project risk.
Frameworks is a more ambitious take on advancing the craft of JS
Ember JS — creator is also from Rails and SproutCore

Libraries: Backbone, Knockout, Spine, CanJS
Frameworks: Ember, AngularJS, Batman, Meteor

more side by side comparisons here:
http://blog.stevensanderson.com/2012/08/01/rich-javascript-applications-the-seven-frameworks-throne-of-js-2012/

All of them must make decisions on how to deal with Views, URL Routing, and Data Storage
If one of them is not built in, argument is that it’s easier to work with 3rd party libraries
If one of them is built in, argument is that integration is more seamless.

Ember (like Rails): We do a lot of magic, but it’s good magic.

String-based vs DOM-based templates

AngularJS — made by guys at Google

String-based templates: use Handlebars.js
DOM-based means more control flow via bindings in your markup and not relying on an external templating library

Server-agnosticism
Batman is designed for Rails 
Meteor does its own thing

The architecture, convention, and tooling in Ember leans towards Rails developers

Quick overview of the different JS technologies:

Backbone
M-V in JS
Most minimal, best known, easy to adopt

Spine
Modified version of Backbone
 
Meteor
Bleeding edge future web framework
Very radical 
Server-side runtime (Node+Mongo) with client-side runtime. WebSockets syncs between client and server. 
Node.js is a framework for server side applications
Mongo is a leading NoSQL open source database
Live deployments each time you edit your code.
Client-side runtimes updated on the fly without losing their state
Beyond conventional web development
Full DB API on the client side—> makes it easier to make dynamic websites
Don’t have to deal with callbacks anymore
An Ecosystem of packages

Internet has latency—> it can take awhile for your DB to update your screen 

Ember
Built by guys from jQuery and Rails
What you need to build an “ambitious” web application
Biggest FM in terms of functionality and code size
Very sophisticated, very opinionated
Design inspired by Rails and Cocoa
Will supply project templates for Rails

Sites using this: NPR

AngularJS
Developed by Google, internally used by them
No impact on your server architecture or file layout
     Doesn’t need to control the whole page: can work on a section of your page
Combination of what browsers do today and what they will do natively in a few years
     Declarative binding and observability —> in a few years

Knockout
Model-View-ViewModel
Focused on rich UIs
Not opinionated on URL routing or data access
Won’t impact server architecture or file layout
Doesn’t need to control the whole page

Batman
For people who use Rails and CoffeeScript
Very opinionated, MUST follow conventions
Full-stack framework with pretty rich models, views, controllers, and routing
DOM-based templating

CanJS
Not very well known

### Non-JS Frameworks 

Ahhh there are so many of them! Play? Sinatra? Ruby on Rails? What to learn?

### What to use?

Which one to choose?
Scope: Are you starting from scratch and want a pre-prepared architecture to guide you?
Or do you prefer to pick your own combinations of patterns and libraries?
Design aesthetic: Do you like doing it?






