---
layout: post
title: "Devise and CanCan"
date: 2014-02-07 13:26:15 -0500
comments: true
categories: 
---

This week I will be talking about making an app that uses Devise for authentication with ActiveRecord and SQLite for a database. I will also be using Test Driven Development (TDD), so I will be including RSpec and Cucumber as well.

##Background:

Devise is a ready made authentication and user managment gem. RSpec is a popular framework for unit testing and Cucumber is used for integration testing and Behavior Driven Development (BDD). This combination of basic gems is the foundation for lots of real-world Rails applications, which is why I'm starting with them. Professional grade applications use TDD and BDD methodologies so I hope as I continue my study of Rails I can incorporate them into my applications and they will be become second nature (hopefully). 
The basic function of Devise is to let you sign up a new user and create an account for them to store in your database. Devise will also require a visitor to login before allowing access to an application. RSpec lets you test your code so it won't break after you ship it. Cucumber lets you figure out if the app's specs work as expected. It will test the app from the point of view of the user. 

Tips and Tricks I learned this week:

How to create a specific gemset:

```
	$ rvm use ruby-2.0.0@rails3-devise-rspec-cucumber --create
	$ gem install rails
```

This is very helpful. It will automatically put you in the gemset that belongs to that project. 

```
	$ echo "ruby-2.0.0" > .ruby-version
	$ echo "rails3-devise-rspec-cucumber" > .ruby-gemset
```

Let me stress that Devise provides *authentication*. This makes sure that the app securely identifies users and makes sure the user is really who they are. Devise also provides user management and implements features to let the user sign up to create/edit an account.

Devise does not provide *authorization*. Authorization determines if an authenticated user should have access to the secured resources. Once you've authenticated a user, you can use CanCan to limit access to users to certain types of content on your site.

CanCan is a popular gem for authorization. 

Related apps I've made:

* An app that uses Devise for authentication with a MongoDB datastore

	* Install Mongo on your computer-> most popular NoSQL db
	* Use -T and -O to skip Test::Unit and Active::Record files
	* Use cucumber-rails generator to set up files needed for cucumber
	* Capybara specifies Capybara instead of default Webrat for acceptance testing
	* rspec enables RSpec matchers for your step definitions 
	* if you used -o flag, the --skip-database option allows Cucumber generator to go without a database.ymp file
	* Need a db cleaner to reset your app db for testing 
	* Check how many instances of mongo are running: ps -ax | grep mongo

```
	$ rails generate cucumber:install --capybara --rspec --skip-database
```



