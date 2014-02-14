---
layout: post
title: "Week Two: RESTful Microframework in Ruby"
date: 2014-02-07 13:26:15 -0500
comments: true
categories: 
---

I decided to implement my knowledge of Ruby that I learned this week by creating a small RESTful microframework in Ruby. Rails employs RESTful principles so I thought that would also be a good way to start thinking about that architectural pattern. It was also a good way to get introduced to different Ruby libraries. 

Step 1: Use socket to build a simple webserver in Ruby

	require "socket"
 
	webserver = TCPServer.new('localhost', 2000)
	while (session = webserver.accept)
  	session.write(Time.now)
  	session.print("Hello World!")
  	session.close
	end

The socket library provides specific classes for handling common transports as well as a generic interface. 

Awesome! Now that I've made a very simple web server in Ruby I need to make it RESTful. 

Resource

REST is all about resources, so I'm starting with the resource type. In REST, we interact with a resource using HTTP methods. An HTTP method will change or query the resource's state, and the resource will respond with a status code and a potential body. 

I will define a Resource interface that defines the four most common HTTP methods. 

However, Ruby doesn't work that way! Ruby has a lack of interface/class support. 

In Ruby, module is the closer rival to abstract classes. You can't create any instances of the module but you can include it with another class. 

In statically typed languages like Java and C#, Interfaces enfore that the classes have methods at compile time. Since Ruby in a dynamically typed language, this doesn't mean anything. Python and Ruby don't have the concept of an interface. 

Other basic OO concepts such as interfaces, method overloading, and operator overloading are missing. 

Ruby Advantages:
* Everything is an object: primitive types, classes, etc. Easier to write unit tests for. In Java, it's harder to write unit tests for. 
* Modules
* Ruby blocks: blocks of code allow for very concise syntax
* Duck typing and syntactic sugars: allow code to be extremely compact and readable. There's no need for type definition or type casting. Ruby is very expressive and easy to read. Java is a lot more verbose than Ruby. 

Java Advantages:
* Performance
* Multi-threading and concurrency
* Interfaces
* IDE Support: becuase of the dynamic nature of Ruby, IDE cannot help much in this sense. Without an extensive test suite it can be really hard to extend/modify an old Ruby project. 


