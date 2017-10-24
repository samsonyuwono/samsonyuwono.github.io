---
layout: post
title:      "Adding J Query to my CRM Rails App"
date:       2017-10-24 11:44:20 -0400
permalink:  adding_j_query_to_my_crm_rails_app
---


After an eventful offseason, the NBA season is finally upon us! This was the year that my Celtics were finally coming together to make a championship run.

Then five minutes into the first quarter, this happened.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/Hkzh1"><a href="//imgur.com/Hkzh1"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

At this point. you're probably wondering why the hell I'm writing about basketball for my blog about programming but bear with me.

Upon successful completion of my Ruby on Rails project, I was riding high. Since Javascript was my first language I flew through this portion of the course.

Once I got deeper into templating and AJAX, I hit a huge roadblock in terms of my comfort with the material. I am in no way equating this to the horrific injury suffered by Gordon Hayward on opening night. 

What I would equate this to was my experience as a Celtic's fan. I experienced initial elation that quickly turned into deflation 

But fear not, through experimentation and some Googling, I have completed another portfolio project. In this post, I will outline the major requirements and what I did to achieve them.

All of the jQuery functions/actions are located within the `companies.js` file. In addtion, I added html to my company index and show page to make it acessible to the functions within `companies.js`


**1. Include an index resource rendered using jQuery and an Active Model Serialization JSON backend.**
In the company index page, I built a drop down button that allows a user to view all of a company's leads information.


<blockquote class="imgur-embed-pub" lang="en" data-id="a/TDFW7"><a href="//imgur.com/TDFW7"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

I achieved this by creating a `moreInfo` function that used jQuery `GET`  to acquire all of a company's leads information. Then, I accessed the DOM in the company index page which allowed the drop down button to work.

**2. Include a show resource rendered using jQuery and an Active Model Serialization JSON backend.**

For this requirement, I decided to build a "Next" button on my company show page. This next button allows a user to sift through their current accounts.

This requirement was more complicated than I anticipated. There were also a lot of moving parts that were needed to achieve this requirement. I had to render each show page to look and act like the original landing page the user started on.

On the Rails side, I added logic for "Next" in my user model and an action within my `companies_controller.rb` file.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/GI7JF"><a href="//imgur.com/GI7JF"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

<blockquote class="imgur-embed-pub" lang="en" data-id="a/eGrzN"><a href="//imgur.com/eGrzN"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

The two key functions that does most of the work in `companies.js` would be `nextCompany` and `updateView` . This is demonstrated below.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/IJ4dA"><a href="//imgur.com/IJ4dA"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

<blockquote class="imgur-embed-pub" lang="en" data-id="a/msv75"><a href="//imgur.com/msv75"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>


**3. Use your Rails API and a form to create a resource and render the response without a page refresh.**
Each company show page allows a user to add comments. For example, the real world application for this would be to update the status of an account.

In order to achieve this requirement, I created a new form for comments within the company show page. Along with this, I built an area that renders all comments.

The function `createNewComments` in `companies.js` accesses the DOM and appends new comments to my company show page. 

<blockquote class="imgur-embed-pub" lang="en" data-id="a/njtfD"><a href="//imgur.com/njtfD"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

Although I have met all the requirements for this project, my to-do list is below. 

1. Add CSS and images to make my project visually appealing
2. Make each lead in the drop down menu on company index clickable. 
3. Build a previous button that allows a user to click back on a previously viewed company

The to-do list is not defnitive. I anticipate that I will add more to it when I achieve some of the above.




