---
layout: post
title:  "Rails: How to add custom fields to Devise"
date:   2017-08-24 15:46:02 -0400
---


In a nutshell, Devise is a Rails engine that provides a lot of authentication needs. It has its own views, controllers, and defines it's own routes.

![](http://imgur.com/a/XtRSU)

The view above for Devise's sign up page is provided by running `$ rails generate devise:views users`

When I started my Rails project with Devise, I initially thought that it would be a matter of inserting my custom field to the sign up views page and adjusting accordingly. 

I was very wrong in that assumption and within this blog post I am going to provide a quick step by step walkthrough on how to add custom fields to your Devise pages. My intention is to provide a concise guide to this simple process.

**Step 1**
Go to `config/initializers/devise.rb` 
Uncomment the line below and change to "true".
<blockquote class="imgur-embed-pub" lang="en" data-id="a/81KpW"><a href="//imgur.com/81KpW"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

<blockquote class="imgur-embed-pub" lang="en" data-id="a/krjdW"><a href="//imgur.com/krjdW"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

**Step 2**

In this step, we will create a new migration. 
`rails generate migration add_username_to_users username:string`

Fill out your generated DB file with your desired fields similar to the image below. Migrate your new file with `rake db:migrate` after the file has been filled out.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/ItOtX"><a href="//imgur.com/ItOtX"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Note: Do not try to add your custom columns in your initial Devise migration, it will not work.

**Step 3**

Go to `app/views/users/registration/new.html.erb` or `app/views/users/registration/edit.html.erb`. From here you can now add your custom fields to your sign up or edit form.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/Tfmia"><a href="//imgur.com/Tfmia"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Your sign up page should look something like the image below.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/2phWx"><a href="//imgur.com/2phWx"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

That's it! You now have the ability to add custom fields to your user sign up and edit pages. 







