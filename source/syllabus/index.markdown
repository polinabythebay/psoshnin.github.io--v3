---
layout: page
title: "syllabus"
date: 2014-01-29 23:32
comments: true
sharing: true
footer: true
---
<a name="return"></a>
Independent Study Proposal

Web Development Studio: Ruby on Rails

Spring 2014

Wellesley College

Student: Polina Soshnin

Faculty Advisor: Jean Herbst 

[Objective](#objective)

[Goals](#goals)

[Overview](#overview)

[Course Materials](#materials)

| [Week 1](#week1) | [Week 2](#week2) | [Week 3](#week3) | [Week 4](#week4) | [Week 5](#week5) | [Week 6](#week6) |

| [Week 7](#week7) | [Week 8](#week8) | [Week 9](#week9) | [Week 10](#week10) | [Week 11](#week11) | [Weeks 12-15](#week12-15) |

[Additional Resources](#resources)

----------------------------------------------------------------------------------------------------------------------------
<a name="objective"></a>**Objective** [Return to top](#return)

My goal is to gain competency and knowledge of best practices in web development by learning and implementing a web development framework. However, it can take hours, days, and weeks to become proficient in the best practices of a specific framework even for experienced developers. This is why I would like to design an independent study where I can devote time to doing so. Why do I want to teach myself Rails specifically? A few reasons: 

* Ruby on Rails is an open-source web framework based on the Ruby programming language. 
* Rails is a database-agnostic MVC framework that chooses convention over configuration, which means that it's strongly opinionated when it comes to architectural decisions, naming conventions, paths and patterns.
* Rails is a full stack web application: it includes libraries to manage frontend code, supports SASS and CoffeeScript, and does not need an external tool to manage compiling. It also includes a very opinionated workflow. 
* Rails’ structure makes it easy to accommodate change. Rails is particularly good at restructuring your application flow, reusing components in a simple way.
* Rails can easily be extended with a wide variety of external libraries, distributed through Rubygems. 
It implements other best practices and methodologies in web development: TDD, REST, and DRY are among them. 

To summarize, Rails is a powerful web development framework that lets you be more productive when working on complex projects. 

----------------------------------------------------------------------------------------------------------------------------
<a name="goals"></a>**Course goals** [Return to top](#return)

By the end of the semester, through coursework and projects I aim to have a competent knowledge of: 

* **Ruby**, including but not limited to: Classes, methods, types, flow control, I/O, modules, Exceptions, Testing, Gems
* **Ruby on Rails**, including but not limited to: MVC model, Active Record, Action Controller, Action View, Action Pack, Testing, Routes, Filters/Callbacks, Debugging, Ajax, Action Mailer, Web Services and XML, Extending Rails, Benchmarking and performance, Deployment
* Exposure to other web technologies: HTML/CSS/Javascript etc. 
* **Git** and **Github**: Use revision control and keep all course repositories on github
* **Heroku**: understand the different Rails servers (Thin vs Unicorn) for deployment 
* Test-driven-development
* Behavior-driven-development
* **Product Planning**: user stories, use cases, wireframes, and mockups
* Exposure to web **APIs**: Twitter, Gmail, Google Maps, MailChimp, Stripe, etc. 

----------------------------------------------------------------------------------------------------------------------------
<a name="overview"></a>**Course overview** [Return to top](#return)

**Weeks 1-8**: Fundamentals of Ruby and Ruby on Rails

**Weeks 9-11**: Build a payments site using Stripe

**Weeks 12-15**: Extend site and/or work on a project of choice implementing gems of choice 

----------------------------------------------------------------------------------------------------------------------------
<a name="materials"></a>**Main Course materials** [Return to top](#return)

*Learn Web Development with Rails* by Michael Hartl

*Learn Ruby on Rails* by Daniel Kehoe

*Mastering Modern Payments: Using Stripe with Rails* by Pete Keen

*The Ruby Toolbox* https://www.ruby-toolbox.com/

*CodeQuizzes* http://www.codequizzes.com/

----------------------------------------------------------------------------------------------------------------------------
**SCHEDULE** (Tentative, subject to change)

<a name="week1"></a>**Week One**: Setup [Return to top](#return)

Setup blog and course

Set up blog using Octopress that is made with Jekyll, a static site generator made with Rails (so I can use Rails to blog about Rails!)

Host blog on github, track blogs and changes on github

Name of blog: http://polina.io/

Blog via Octopress: http://octopress.org/docs/blogging/

----------------------------------------------------------------------------------------------------------------------------

<a name="week2"></a>**Week Two**: Ruby fundamentals [Return to top](#return)

Exercises

Work through Try Ruby Exercises http://tryruby.org/levels/1/challenges/4

Learn Ruby the Hard Way http://ruby.learncodethehardway.org/book/

Rubymonk: metaprogramming and common ruby methods https://rubymonk.com/

Code Academy http://www.codecademy.com/tracks/ruby

Ruby Koans http://rubykoans.com/

Quizzes

* Ruby Array Quiz 
* Hash quiz 
* Object Oriented Programming 
* More OOP 
* Inheritance 
* Object Oriented Design 
* Code Blocks 

Homework

* RESTful micro framework in Ruby 
* Write Blog Post
* Update Github

----------------------------------------------------------------------------------------------------------------------------

<a name="week3"></a>**Week three**: Rails fundamentals [Return to top](#return)

Exercises

Chapters 1-2 *Learn Web Development with Rails*

* From zero to deploy: Version Control with GIT, deploying with Heroku
* A demo app: planning the application, the Users resource, the Microposts resource

Chapters 1-8 *Learn Rails*

Jeffrey's introduction to Rails http://net.tutsplus.com/tutorials/ruby/the-best-way-to-learn-ruby-on-rails/

Rails for Zombies
https://www.codeschool.com/courses/rails-for-zombies-redux

Rails intro screen cast http://net.tutsplus.com/tutorials/ruby/the-intro-to-rails-screencast-i-wish-i-had/

Git Immersion http://gitimmersion.com/

Quizzes

* Learning Unix for OS X
* Basic Git Commands 
* Basic Git 
* Git Rebasing 
* Git branch off a branch 
* Git interactive rebasing 
 
Homework

* Tiny Static Site generator in Ruby 
* App from *Learn Rails*: Contact form, save to Google Spreadsheet 
* Update Github
* Write Blog Post

----------------------------------------------------------------------------------------------------------------------------

<a name="week4"></a>**Week Four**: Rails Fundamentals [Return to top](#return)

Exercises

Chapters 3-4 *Learn Web Development with Rails*

* Static Pages
* Rails Flavored Ruby

Chapters 9-28 *Learn Rails*

Homework

* Devise for authentication with ActiveRecord and SQLite for a database
* Devise for authentication with a MongoDB datastore
* Continue working on static site generator if not finished
* Update Github
* Write Blog Post

----------------------------------------------------------------------------------------------------------------------------

<a name="week5"></a>**Week Five**: Rails Fundamentals [Return to top](#return)

Exercises

Chapters 5-6 *Learn Web Development with Rails*

* Filling the Layout
* Site navigation
* Bootstrap, CSS
* Partials
* Sass and asset pipeline
* Layout links
* User signup: first step
* Modeling Users
* User model
* User validations
* Adding a secure password

Homework

* OmniAuth for authentication with a MongoDB datastore
* Base-camp style subdomains with Devise and MongoDB
* Update GitHub
* Write Blog Post

Additional Homework

* Make a to-do list app with Rails

----------------------------------------------------------------------------------------------------------------------------

<a name="week6"></a>**Week Six**: Rails Fundamentals [Return to top](#return)

Exercises

Chapters 7-8 *Learn Web Development with Rails*

* Sign up
* Showing Users
* Signup form
* Signup failure
* Signup success
* Sign in, Sign out
* Sessions and sign in failure
* Sign in success
* Introduction to Cucumber

Homework

* Devise for authentication and CanCan for authorization
* Integrating Rails 4.0 and Twitter Bootstrap 3.0
* Update GitHub
* Write Blog Post

----------------------------------------------------------------------------------------------------------------------------

<a name="week7"></a>**Week Seven**: Rails Fundamentals [Return to top](#return)

Exercises

Chapters 9-10 *Learn Web Development with Rails*

* Updating, showing, and deleting users
* Updating users
* Authorization
* Showing all users
* Deleting users
* Using Microposts
* A micropost model
* Showing microposts
* Manipulating microposts

Homework

* Application for a startup prelaunch signup site
* Update GitHub
* Write BlogPost

----------------------------------------------------------------------------------------------------------------------------

<a name="week8"></a>**Week Eight**: Finishing up Rails Fundamentals [Return to top](#return)

Exercises

Chapter 11 *Learn Web Development with Rails*

* The Relationship model
* A web interface for following users
* The status feed
* Conclusion

Homework

* Site with subscription billing using Stripe
* Site with subscription billing using Recurly
* Update GitHub
* Write Blog Post

Additional Homework

* Create scaled down reddit clone in rails
* Recreate Twitter in rails
----------------------------------------------------------------------------------------------------------------------------

<a name="week9"></a>**Week Nine**: Building a payments website [Return to top](#return)

Exercises

Chapters 1-3 *Mastering Modern Payments: Using Stripe with Rails*

* Introduction
* The Simplest Stripe Integration
* Security and PCI Compliance

Homework

* Start payments project 
* Blog
* Update Github

----------------------------------------------------------------------------------------------------------------------------

<a name="week10"></a>**Week Ten**: Building a payments website [Return to top](#return)

Exercises

Chapters 4-6 *Mastering Modern Payments: Using Stripe with Rails*

* Custom Payment forms
* State and History
* Handling Webhooks

Homework

* Work on payments project
* Blog
* Update Github

----------------------------------------------------------------------------------------------------------------------------

<a name="week11"></a>**Week Eleven**: Building a payments website [Return to top](#return)

Exercises

Chapters 7-10 *Mastering Modern Payments: Using Stripe with Rails*

* Processing payments with Background workers
* Subscriptions
* Marketplaces
* Additional Resources

Homework

* Finish/continue payments project
* Blog
* Update Github

----------------------------------------------------------------------------------------------------------------------------

<a name="week12-15"></a>**Weeks 12-15**: Implement popular Gems and test Rails knowledge [Return to top](#return)

Quizzes to test Rails knowledge

* MVC without generators: Create a RESTful model, view, and controller without using any rails generators.
* Nested Resources: Create the model, view, and controller for a nested resource.
* Database Queries : Structure database queries to get specific information from a database efficiently.
* Polymorphism: Make a resource that belongs_to two other resources for nested comments.
* Active Record: Associations, delegation, callbacks, etc.
* Many to Many Relationships : Rails practice problems on has_and_belongs_to_many and has_many :through relationships

The Ruby Toolbox

Choose several of the following areas and create apps with a focus on implementing popular gems in those areas:

* Active Record Plugins
* Background processing
* Code Quality: code metrics
* Communication
* Content Management and Blogging
* CSS
* Data Persistence
* Dev Tools
* Documentation Tools
* Graphics
* HTML and Markups
* Javascript
* Maintenance and monitoring
* Package and depedency management
* Provision, deploy, host
* Rails plugins
* Security
* Testing
* Time and Space
* Web apps, Services, and Interaction

Homework

* Work on project(s)
* Update blog
* Update Github

Optional Quizzes

* Recursion 
* Big O 
* Selectors 
* Inheritance and the cascade 
* Beginning/Intermediate jQuery 

Learn/test Javascript knowledge

* Quiz #1 
* Quiz #2 
* Quiz #3 
* Quiz #4 
* Quiz #5 

----------------------------------------------------------------------------------------------------------------------------

<a name="resources"></a>**Additional Resources** [Return to top](#return)

Books

* Rails3 in Action
* Agile Web Development in Rails
* The Rails Way
* Programming Ruby: The Pragmatic Programmer’s Guide
* The Ruby Programming Language
* Practical Object-Oriented Design in Ruby
* Rails Guides http://guides.rubyonrails.org/getting_started.html
* Ruby Style Guide https://github.com/bbatsov/ruby-style-guide
* Test First http://testfirst.org/learn_ruby
* Design Patterns in Ruby http://designpatternsinruby.com/
* Eloquent Ruby http://eloquentruby.com/
* Well Grounded Rubyist 
* The RSpec Book

Podcasts

* Railscasts
* Ruby5
* The Changelog
* CoderPath
* Software Engineering Radio
* This Developer’s Life
* Pragmatic Podcasts

Meetups

* Boston Ruby Women
* Girl Develop It Boston
* Boston Ruby on Rails
* RailsBridge
* Rails Girls

Hackathons 

* WECode
* PennApps
* Hack Beantown
* MIT ID Hack
* Boston I/0

Community

* Hacker News
* Reddit
* Stack Overflow
* Confreaks http://confreaks.com/
* Green Ruby http://greenruby.org/
* Project Euler
* HackerRank
* Rails Best Practices http://railsbest.com/
* Ready Set Rails http://www.readysetrails.com/
* Rubies in the Rough http://subinterest.com/rubies-in-the-rough
* General Assembly: Ruby on rails for developers https://github.com/generalassembly/ga-ruby-on-rails-for-devs
* Ruby Quiz http://rubyquiz.com/
* Ruby Rogues http://rubyrogues.com/
* Ruby Stack http://bitnami.com/stack/ruby
* The Ruby Game http://www.therubygame.com/challenges/distressed-ducks/submissions



















