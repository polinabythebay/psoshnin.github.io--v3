---
layout: page
title: "glossary"
date: 2014-01-31 15:10
comments: true
sharing: true
footer: true
---
<a name="return"></a>
This is where I will keep a running list of terms and concepts for personal reference. The list is by all means not exhaustive and isn't limited to Rails/Web Development. There are really awesome resources online if you're looking for a comprehensive list like [Webopedia](http://www.webopedia.com/) or [Wikipedia](http://www.wikipedia.org/).

[Ruby on Rails](#rails) | [Product Planning](#pm) | [Web Development](#webdev)

##Some basic Internet and Web terms 

* **API**: 
* **Ajax**: Originally asynchronous JavaScript and XML. Now refers more broadly to web development where methods within a page call back to the server and make smaller changes to a page rather than calling for a complete refresh every time.
* **Boolean Logic**: system of standardized operators used to connect search terms. Will include AND, OR, NOT, and sometimes NEAR. 
* **Basecamp**: A collaboration tool developed by 37signals and DHH. DHH realized that the underlying framework could be used for a lot of other projects, and that became the foundation of Rails. 
* **Browse/browser**: browsing a page is guessing which words and links on the page pertain to your interests. It's the opposite of searching. Browsers enable you to view web pages and other documents on the internet. They translate HTML encoded files into text, images, sounds, etc. Common browsers include Firefox, Internet Explorer, Mozilla, Safari, Opera, and Chrome. 
* **Cache**: Space where web pages you have visited are stored in your computer. When you use GO, BACK, or any means to revisit a document, the browser first checks to see if it is in the cache and will retrieve it from there because it's much faster than retrieving it from the server.
* **Cached Link**: In search engines, like Google, Bing, and Yahoo! Search, there is usually a cached link that lets you view the version of a page that the search engine has stored in a database. The live page on the web may differ that the cached version, since the cached version dates to whenever the search engine's spider last visited the page and detected the modified content. You can use the cached link to see when a page was last crawled. 
* **Case sensitive**: Most search tools are not case sensitive. Passwords are. 
* **CGI**: Common Gateway Interface. Most common way for web programs to dynamically interact with users. A lot of search boxes/other applications that load a page tailored to a user's search terms rely on CGI to process data once it's submitted, pass it to a background program(Javascript, Java, whathaveyou), and then integrate the response into the display using HTML.
* **Cloud Computing**: distributed computing over a network. It lets one run an app or program on many connected computers at the same time.
* **Cookie**: A message from a web server that is sent and stored by your browser on your computer. When your computer talks to the original server, the cookie is sent back, allowing it to respond to you according to its contents. Cookies can provide customized web pages according to a profile of your interests. Chrome autofilling in your name and address on a form is from a cookie. 
* **Custom Search Engine (CSE)***: This is a Google service. You can create a custom search engine that is made to search within a group of websites or pages. 
* **DOM**: Document Object Model. Standard API for manipulating HTML documents in a web browser. 
* **Top Level Domain (TLD)**: This is a heirarchical scheme that is used to indicate a category of a webpage from the network. Common domains are .edu (education), .gov (the Feds, people), .net (network related), .com (commerical), .org (nonprofit). There are, of course, lots of others. 
* **Domain Name, Domain Name Server, DNS Entry**: The domain name gives you who "published" a page and made it public by putting it on the web. The domain name is translated in huge tables that are standardized across the internet into numeric IP addresses that are unique to the host computer. These tables are maintained by Domain Name Servers. When you ask the browser to find a URL, the browser consults the table on the domain name server that is connected to that computer. 
* **Download**: Copy something from the primary source to a peripheral one. 
* **Fat client**: Heavy/rich/thick client. A computer in client-server architecture that provides functionality independent of the central server. 
* **Freshness**: How up-to-date a search engine database is. This can depend on how often the spiders recirculate around the web and update their copies of web pages and discover new ones. 
* **Header**: Top portion of HTML source code behind web pages. It contains the Title, description, key word fields, and other things web page authors use to describe a page. Need to click view source to see this.
* **Host**: Computer that provides web-documents to clients or users. 
* **HTML**: Hypertext Markup Language. It's imbedded in the source docs behind all web docs. Browsers are made to read HTML for display. 
* **Hypertext**: 
* **Internet**: interconnected networks that use TCP/IP protocols and evolved from the ARPANET of the late 60s/70s. An intranet is a private network inside a company or org. An intranet could be on the Internet or just be a network.
* **IP Address**: Internet protocol number/address. Unique number of 4 parts separated by dots. Ex. 185.112.23.1. Every machine on the Internet has a unique IP address. 
* **ISP**: Internet service provider. Company that sells internet connections. You can get faster, more expensive internet via cable/DSL.
* **Java**: A network-oriented programming language invented by Sun Microsystems. You can write programs that can be safely downloaded to your computer via Internet. Small Java programs are called Applets. They can let web pages include stuff like animations and calculators.
* **Link**: URL embedded in another document. Link rot is the frustrating problem caused by constantly changing URLs. URLs can change frequently when docs are moved to new computers, file structure on computer is reorganized, sites are discontinued, etc. 
* **Listservers**: Allows you to subscribe and recieve 
* **Saas**: software as a service. A software delivery model in which software/associated data are hosted on the cloud. It's typically accessed by users using a thin client via a web browser. It's a common model for delivery for many business applications. Think office and messaging, accounting, enterprise resource, content management, etc. 
* **Thin client**: Lean/zero/slim client. Computer or program that relies heavily on another computer/server to fulfill its computational roles. 
* **.shtml**: file name extension that identifies web pages containing SSI commands.
* **URL**: uniform resource locator. It's the unique address of any web document. 
* **XHTML**: hybrid of XML and HTML. 
* **XML**: Extensible markup language. 

<a name="rails"></a>
##Ruby on Rails
[Return to top](#return)

* **37 Signals**: the company where Rails was born, emerging from their Basecamp product.
* **Acceptance Testing**: test cases that are written in a way that describes a use case. Cucumber is a good tool for acceptance testing. You work with your stake holder to develop tests that represent use cases. When the test is complete the feature should be accepted. This kind of testing is focused around the people outside the code development accepting features.
* **Application servers**: Thin, Mongrel, Passenger, Unicorn, Pow. They interact with your Ruby code and respond to requests. They are integrated with web servers like Nginx and Apache to serve your application on the internet.
* **Authentication**: process of matching credentials to a person and verifying them. Purely about identifying who the user is-- not what they can do. Devise is a good athentication library/gem for that.
* **ActionController**: The part of the Rails library that directly interacts with incoming HTTP requests, including routing, parameter passing, session management, and deciding how to render a response. Controller objects are how a Rails developer interacts with ActionController.
* **ActionMailer**: The part of the Rails library that manages incoming and outgoing email.
* **ActionPack**: Combination of ActionController and ActionView, which provides a complete package for dealing with and responding to HTTP requests.
* **ActionView**: generates responses to HTTP requests
* **Authorization**: process of determining what a specific user can do. Usually involves permission or role based sytems. CanCan is a good authorization library for that.
* **Active Record**: ORM tool to abstract database handling. Implementation of Active Record architectural pattern. Handles mapping between the database and Ruby classes. This is pretty much the foundation of Rails. 
* **Active Resource**: like an Active Record for REST based web-services. Provides a wrapper around REST actions. Can act like a transparent proxy between a business entity and a REST based service. 
* **Active Support**: set of utility classes and standard library extensions that are useful. They range from caching to dates, time zones, text etc. 
* **acts_as*: common naming convention in Rails, typically with plug-ins, to indicate that part of a model operates using code that is elsewhere. 
* **aggregation**: 
* **adapter**: code the connects ActiveRecord to a specific database.
* **Builder**: an API used to generate XML files from Ruby objects.
* **Bundler**: manages gem dependencies in a repeatable way across multiple machines. Automatically looks for and installs/updates all gems needed by the application when it is deployed on a machine. It reads a Gemfile and calculates a set of version requirements to make all specific gems live happily ever after. It will prevent version conflicts and the infamous 'gem already activated error'. It does not require libraries, simply just makes them available. It can be used outside of rails-- you can use it when you do any ruby work.
* **Capistrano**: tool for executing command on groups of servers over SSH. Used mainly in deploying web applications and is capable or recognizing different types of server environments (staging vs production etc). You can easily write your own tasks similar to writing a rake task. It's the preferred way to deploy Rails applications. 
* **Capybara**: gem designed to provide an abstraction layer between different browser drivers. Used in integration testing to interact with the web server. Provides an API to navigate between pages, click buttons, fill in forms, and other user interactions. Has adapters for many different browser drivers. Some drivers include Selenium, rack-test, and webrat.
* **Compass**: library built around SASS abstractions. Provides mixins for many common things like styling buttons and forms. It's easy to extend and comes with many built in functions. Blueprint CSS framework is bundled by default.
* **CoffeeScript**: A little language that compiles into Javascripty. It's really popular and the default method of writing Javascript in a Rails Application.
* **Controller**: collection of actions in an MVC application. Routes direct a request to a Controller's action. From there, the controller is used to manage the user's request and determine with business logic is to be executed in an application.
* **Cucumber**: Test framework for creating plain english acceptance tests. Used for integration testing web applications. Test suite ofeten used in Continuous Integration. It uses a language called Gherkin to parse files into lines and match them with regular expressions. The regular expressions are then matched with code blocks. Your test code lives in these blocks. Lets you describe how software should behave in plain text. Text is written in DSL and serves as documentation, automated tests and development aid. Cucumber and RSpec are the main tools used for BDD in Rails projects. Cucumber tests are divided up into "Feature" files. Each "Feature" has many "scenarios". Features are like use cases. Scenarios are different permutations of that use case. 
* **duck typing**: A way of determining what type an object is by looking at what it contains and how it behaves. It's built into the Ruby language. 
* **DHH**: David Heinemeier Hansson, creator of Rails and lead developer. loudthinking.com
* **DSL**: Domain specific language dedicated to a particular problem or solution. Ex: Cucumber, Rake, Haml, etc. They are crafted to solve one or more problems very eloquently and nothing more. They are usually wrappers around more complicated methods that make it easier to express the intent of the underlying code from a programmer's perspective.
* **Edge Rails**: The latest (and sometimes greatest) version of Rails. Exciting for advanced developers, potentially explosive for beginners. 
* **ERB**: Embedded Ruby. Simple and powerful templating system for Ruby. Part of the Ruby core and allows one to place ruby within other files. 
* **Factories**: Factory Girl & Machinist: gem that is useful for creating object factories in an automated fashion. Useful in testing or even for populating an application when deployed. Used in test suites and population scripts. They provide a default set of attributes and allow programmers to specify the attributes they care about at creation time.
* **Gem**: a Ruby gem is a package. They're like an app-store for your development needs where a ton of awesome gems are freely available! The number of awesome useful gems gives Ruby developers a huge advantage over other frameworks.
* **Generate Command**: used as a shortcut for installing and creating models, controllers, actions, routes, and initializers to save the developer time when creating an application. Rails provides a set of templates that can be used to generate code. Gems can also provide their own generators.
* **Gherkin**: DSL that emerged from the Cucumber project. It's designed to succinctly describe behavoir. 
* **Git**: free open source distributed version control system. Written by Linus Torvalds. Used alongside Github. Each user has a complete copy of the repository. Most developers use github exlusively. 
* **Haml**: HTML abstraction language. Functions as a replacement for PHP, ASP, and ERB. It's great for structuring documents and horrible to content. You can also include ruby code inside templates.
* **Heroku**: cloud based platform PaaS, had one of the first to have Ruby on Rails support.
* **jQuery**: Javascript framework of choice for web developers everywhere. Fast framework that leverages CSS style selectors to allow developers to traverse, animate, and handle events in the HTML DOM while abstracting browser specific quirks as far as possible. It's the default Javascript framework used in Rails 3 applications.
* **Layout**: outer aspects of HTML document. Layout includes the header, nagivation, footer, but not main content of a page.
* **lighttpd*: web server designed to be smaller and more efficient than Apache. If you want to run Rails through FastCGI, lighttpd is a good option.
* **Metaprogramming**: dynamically generating code at runtime. It's why Rails feels the way it does. ActiveRecord associations to dynamically add methods to your classes based on how to declare. It's possible in Ruby because Ruby is a dynamic language interpreted at run time.
* **Memcached**: distributed open source caching system. In-memory key-value store for small chunks of arbitrary data (strings, objects) from the results of database call, API calls, and page rendering. It is a generic store and can be used in any situation where caching is needed. Other object stores: Redis.
* **Matz**: Yukihiro Matsumoto, creator and maintainer of Ruby. 
* **MINASWAN**: "Matz is nice, so we are nice". Key principle of Ruby culture. 
* **Merb**: MVC framework, but lighter barebones version. Compare to Rails and Sinatra. 
* **Migration**: a database migration. It's a set of change to the database that can be executed and reversed to provide consistency to the database structure, like adding a column or table. Migrations are marked with a timestamp so each db knows the most recent change that was made.
* **Model**: representation of a database table. used for storing, querying, and manipulating data in application.
* **MVC**: Model, View, Controller. Software pattern that separates the representation of information from the user's interaction with it. Generally, the controller determines which models to interact with and which views are used to display the data.
* **Open classes/monkey patching**: Open classes is a feature of Ruby. Lets you open and add methods to existing classes. Active Support library uses this feature to add a lot of its helper functions on the ruby core classes.
* **Page**: completed HTML document that is returned from a web application and displayed in the user's browser. Typically corresponds to a specific URL on a web site/application. 
* **Paperclip**: complete and easy file attachment library for active record. Provides validation features based on the properties of the file like size, type, etc. Has basic image manipulation like creating thumbnails etc. Dependency: ImageMagick: awesome image manipulation libary.
* **Prototype**: Javascript framework that helps with dynamic web applications. Originally default javascript framework.
* **Rack**: Gem that provides a simple interface between a web-server and the Ruby web framework. Rack is used in Rails, Sinatra, and Merb.
* **Rake**: the Ruby version of 'make' but more developer friendly. Uses Ruby syntax instead of XML files or makefile syntax to define tasks. It's a software task management tool that allows you to define tasks that are often repeated such as running database migrations and deploying code to servers.
* **Request**: When a user's browser asks for a response from your web application.
* **Resource**: An object you can create, read, update, and delete (CRUD). Usually referenced as part of RESTful application design.
* **REST (Representational State Transfer)**: set of principles that define how Web standards, such as HTTP and URIs, are supposed to be used. It's more of a concept than an abstraction. Rails exploits REST concepts. A style of architecture for distributed systems such as the web. Designed around the idea that an application has designated objects that you can create, read, update, and delete (CRUD).
* **RJS**: Ruby Javascript. Ruby helper used to generate Javascript to decorate HTML pages. Mainly used in AJAX calls. This violates UJS bc it uses Ruby helpers to generate Javascript to dump into HTML attributes.
* **Routes**: URLs that your web application responds to.
* **Routing**: deals with translation of a URL request to a specific action in the application. In Rails it's the job of the Router to recognize URLs, avoiding the need for hardcoded strings in Views. A decision making process of a web app that handles incoming requests and determines which actions should happen as the result of the request.
* **RSpec**: Behavoir Driven tool for Ruby programmers. It helps you do the RDD part, focusing on the documentation and design aspects of TDD. It uses a DSL to simplify design and implementation tests. It's a unit testing framework. It's based around the idea that test should describe behavior of classes in an English like way. Test files are called "specs". Spec files are divided into "examples".
* **Ruby**: dynamic, reflective, general-purpose object-oriented programming language created by Yukihiro Matsomoto in 1995.
* **Ruby Debug**: debugger for ruby applications. 
* **RVM**: use to install manage, and work with muliple versions of Ruby and multiple gemsets. It's a set of bash script designed to allow you to switch out Ruby interpreters on the fly. Makes it very easy to install different implementations.
* **SASS & SCSS**: CSS abstraction languages. They are compiled down to CSS. They allow you to use variables, modules, and include other files. Cleans up CSS syntax significantly. Lets developers spend their time writing more readable code without having to deal with writing plain CSS.
* **Scaffolding**: shortcut in Rails that creates controller, set of actions, views, and routes for resources. Frowned upon by experienced developers.
* **Selenium**: a library that simulates user interaction with a browser. It runs the full browser. It works best with Firefox, but can also work with Chrome and friends. Commands are sent across as Javascript which the browser evaluates to complete each action. It's the most complete solution for simulating a user for your web app.
* **Sinatra**: minimalist web framework.
* **Test::Unit**: Default testing library in Ruby. Not really used-- people use BDD style tools like RSpec.
* **UJS**: This is separation of Church and State. Unobstructive Javascript. A general approach to use Javascript in web pages. It separates Javascript from the HTML. Putting Javascript in HTML makes it harder to maintain.
	[1] Separation of behavior from the markup: HTML is meant to describe structure of doc and should not contain programmatic elements. 
	[2] Should not pollute the global namespace. UJS Code should add as little as possible to the global object or global namespace of the environment in which it runs.
	[3] Degrade graceflly: if the browser rendering the document does not have the capability needed then the code should be able to degrade gracefully without break the rest of the application.
* **Vim**: text editor popular among the Ruby folk. I should probably look into this.
* **View**: describes HTML response of a request but doesn't include the outer HTML layout of the page, simply the HTML that is unique to the page.
* **Web servers**: Apache, nginx, Lighthttpd, Thin. Thin is both a web and application server. PaaS providers like Heroku have allowed this part of web app development to be abstracted out.
* **Webrat**: headless browser that is used in web app testing. It lets you run in browser tests with associated overhead of actually instantiating a browser. It does not execute javascript but is great for doing tests for simple websites without much JS interactions. It's the most basic driver and perfect for interacting with simple websites. It's the original headless browser.
* **Will_Paginate**: most popular pagination library for Rails. Also supports Merb and Sinatra. Has varieta of formatting options and can accept an active record object or even a simple array. Very configurable and can be easily extended to do AJAX pagination as well. 

<a name="pm"></a>
##Product Management
[Return to top](#return)

* User stories
* Use cases
* Wireframes
* Mockups

<a name="webdev"></a>
##Web Development
[Return to top](#return)

* **ACID**: Atomicity, Consistency, Isolation, Durability. A set of principles, usually implemented with relational databases and transactions, that are intended to ensure data reliability. Rails is not designed with ACID as a priority, though transactions are available as a plug-in. 
* **Agile**: software development techniques that tend to focus on smaller-scale iterative development rather than top down design and implementation.
* **Benchmark**: code used to determine and compare performance. Generic benchmarks used to test things like CPU performance are the most common usage.
* **BDD**: essentially the same as TDD except you use a different set of tools to express code in terms of user facing behavior. Rspec and Cucumber are part of BDD toolbox.
* **TDD**: method of developing software where requirements are first written as tests. It makes the developer spend more time thinking about the code upfront while providing a solid test suite for the entire application. These tests define actions the software should take and expected results. Once the tests are written, developers can begin to build software to properly return the correct results of each test. The idea behind this is that using TDD lets development be much more consistent when you have a set of tests that all code must run against. Changes to software that break a test quickly show where broken code was introduced.
* **cron**: A unix approach to scheduling tasks that need to run on a regular basis. Cron jobs are managed through the crontab configuration file, and the cron daemon makes sure they get executed as requested. Rails itself doesn't use cron.
* **CVS**: Not an American pharmacy store. Concurrent Versioning System that's used to manage different versions or programs and related files. Rails usually just uses subversion or git.
* **DRY**: Don't repeat yourself: a central principle in Rails development.
* **Firebug**: Firefox plug-in for debugging JavaScript.
* **JSON**: JavaScript Object Notation, a text-based format for exchanging objects. Seen as a programming-oriented complement/competitor to XML. It's also a subset of YAML.
* DDD
* REST
* CoffeeScript
* web framework
* DNS
* ISS
* load balancers
* sticky routing
* round robin
* clustering
* fault tolerance
* server hardware setup
* web farms
* cache farms (memcached win32, velocity)
* SMTP
* MSMQ
* database mail queuing
* n*log(n) sorying algorithm: quick sort, merge sort. pros and cons of both. 
* Big O
* Singleton Design Pattern
* Factory Design Pattern
* Memory (Stack vs Heap)
* Recursion
* Regex
*

<a name="networking"></a>
##Networking 
[Return to top](#return)

* **HTTPS*: encrypted HTML. Hypertext Transfer Protocol over Secure Socket Layer. Works like HTTP except that the web server adds a layer of encryption using public key certificates, it runs on port 443, and browsers are typically more cautious about caching information that arrived over HTTPS.
* sessions
* caching
* state management
* cross site scripting 
* styling
* client side vs server side
* browser support
* HTTP
* get vs post
* cookies
* **FTP**: File transfer protocol. Ability to transfer entire files from one computer to another, for viewing purposes or other. 

<a name="operating systems"></a>
##Operating Systems
[Return to top](#return)

* Processes
* Process Needs
* Threads
* Thread Needs
* Concurrency Issues
* Locks
* Mutexes
* Semaphores
* Monitors
* Deadlock
* Livelock
* Context Switching
* Scheduling
* "modern" concurrency constructs: multi-core, etc

<a name="math"></a>
##Math 
[Return to top](#return)

* basic discrete mathematics: counting problems, probability problems
* combinatorics
* probability 

<a name="algorithms"></a>
##Algorithms
[Return to top](#return)

* Famous classes of NP-Complete problems
* Traveling Salesman
* Knapsack problem
* BFS and DFS
* Inorder, postorder, preorder
* Binary Search
* Merge Sort
* Quick Sort
* Tree Insert/Find/etc

<a name="data structures"></a>
##Data Structures
[Return to top](#return)

* Linked Lists
* Binary Trees
* Tries
* Stacks
* Queues
* Vectors/ArrayLists
* Hash Tables: most important data structure in the history of mankind. Know how to implement one using only arrays

<a name="graphs"></a>
##Graphs
[Return to top](#return)

* ways to represent a graph in memory: objects and pointers, matrix, adjacency list. know the pros and cons of each. 
* Basic graph traversal algorithms: breadth-first search and depth-first search. 
* Computational complexity of graphs, trade-offs, how to implement them in code
* Dijkstra
* A* 

<a name="trees"></a>
##Trees
[Return to top](#return)

* Basic tree construction
* traversal and manipulation algorithms
* binary trees
* n-ary trees
* trie-trees
* types of balanced binary trees: red/black, splay, AVL, how it's implemented

<a name="architecture"></a>
##Architecture
[Return to top](#return)

* Versatility
* Conceptual Integrity
* Independently changeable
* Automatic Propagation
* Buildability
* Growth Accomodation
* Entropy Resistance
* Module
* Dependency
* Process
* Data Access
* Types: Enterprise Applications, Systems, End-user applications, programming languages







