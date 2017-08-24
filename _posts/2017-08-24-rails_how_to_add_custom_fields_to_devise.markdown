---
layout: post
title:  "Rails: How to add custom fields to Devise"
date:   2017-08-24 19:46:01 +0000
---


In a nutshell, Devise is a Rails engine that provides a lot of authentication needs. It has its own views, controllers, and defines it's own routes.

![](http://imgur.com/a/XtRSU)

The view above for Devise's sign up page is provided by running `$ rails generate devise:views users`

When I started my Rails project with Devise, I initially thought that it would be a matter of inserting my custom field to the sign up views page and adjusting accordingly. 

I was very wrong in that assumption and within this blog post I am going to provide a quick step by step walkthrough on how to add custom fields to your Devise pages. 

**Step 1**
Go to `config/initializers/devise.rb` 
Uncomment the line below and change to "true".
![](http://imgur.com/a/81KpW)
![](http://imgur.com/a/krjdW)

**Step 2**

In this step, we will create a new migration. 
`rails generate migration add_username_to_users username:string`

Fill out your generated DB file with your desired fields similar to the image below. Migrate your new file with `rake db:migrate` after the file has been filled out.

![](http://imgur.com/a/ItOtX)

Note: Do not try to add your custom columns in your initial Devise migration, it will not work.

**Step 3**

Go to app/views/users/registration/new.html.erb or app/views/users/registration/edit.html.erb. From here you can now add your custom fields to your sign up or edit form.

![](http://imgur.com/a/Tfmia)

Your sign up page should look similar to the image below.
![](http://imgur.com/a/2phWx)









