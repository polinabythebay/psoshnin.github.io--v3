---
layout: post
title: "Installing Ruby and Rails"
description: ""
category: 
tags: []
---
{% include JB/setup %}

I was told that setting up my development environment for writing Rails apps was going to be one of the trickiest parts of my entire learning experience, and they were right. The process was convoluted enough that I'm making a post out of it to use as a means for documenting the process should I need to redo it in the future. 

The best list of instructions for installing the latest version of Rails (4.1) and Ruby (2.0) for Mac 10.9 Mavericks can be found [here](http://railsapps.github.io/installing-rails.html).

However, what Daniel failed to mention in his installation guide was that you *will* need to also install previous versions of Ruby (1.9.3) and Rails (3.2) in order to successfully complete some of his tutorials. It's also a good exercise in managing different versions of Ruby and Rails for different projects and understanding how RVM works.

So here's what you need to set up your Rails environment. I'm going to assume you are using Mac OSX 10.9 Mavericks.

 * ##### Xcode
This is Apple's development environment. You would use this if you were creating apps for iOS or Mac. Xcode includes a few system libraries that you need for Rails development.

 * ##### Homebrew
Homebrew is a package enviroment for OSX that is really good to have in general when installing packages. It will install most missing system packages that you'll need for Rails.

 * ##### RVM (Ruby Version Manager)
If you're serious about learning Rails development, you will install RVM. It lets you manage different versions of Ruby, Rails, and Gems so you can try out new versions and use different production environments for different applications without having to install/reinstall everything. 

##### Install XCode
* Click and install XCode from the Mac Store (this is large-- it could take awhile)
* Once installed, go to Preferences -> Downloads -> Install Command line tools

##### Install Homebrew and apple-gcc42
This will install the Homebrew package manager and a GCC compiler.


##### Exploring RVM 
This is the structure of RVM. If you type *rvm list* into your terminal it will show you a list of available Ruby versions:

	$ rvm list
	rvm rubies

	=> ruby-1.9.3-p484 [ x86_64 ]
   	   ruby-2.0.0-p353 [ x86_64 ]
 	 * ruby-2.1.0 [ x86_64 ]

	# => - current
	# =* - current && default
	#  * - default

If you want to switch between differeny versions of Ruby, type in *rvm use 2.0.0*:

	$ rvm use 2.0.0
	Using /Users/psoshnin/.rvm/gems/ruby-2.0.0-p353

Type in *rvm list* to see you've switched branches:

	$ rvm list
	rvm rubies

	   ruby-1.9.3-p484 [ x86_64 ]
   	=> ruby-2.0.0-p353 [ x86_64 ]
 	 * ruby-2.1.0 [ x86_64 ]

	# => - current
	# =* - current && default
	#  * - default

In addition to having different versions of Ruby you will also have different gemsets associated with your current Ruby version. Type in *rvm gemset list* to view a list of available gemsets for Ruby 2.0.0.

	$ rvm gemset list
	gemsets for ruby-2.0.0-p353 (found in /Users/psoshnin/.rvm/gems/ruby-2.0.0-p353)
	=>  (default)
		global
		rails-bootstrap

The arrow shows that my default gemset is active. You can see I've created a *rails-bootstrap* gemset for a specific project. Use the command *rvm gemset use global* and *rvm gemset use default* to switch between gemsets.






