---
layout: post
title:  "Making it all come together- My Sinatra Project Blog Post"
date:   2017-07-14 13:10:25 -0400
---


Despite the challenges of the past week, I have finally completed my individual project for Sinatra! I would have to say the most difficult aspect of this project was to put everything we learned about Sinatra together. That list includes but is not limited MVC, Active Record, Sessions, and Forms. 

Summary

For this project, I have decided to create a Workout Program App. On the user side, the goal of this app is to allow the user to add exercises to their daily workout program. Once an exercise is added, the user can view details, edit, or delete a particular exercise.

The Process
The idea to come up with this project was very simple. Keeping up good habits including exercise has always been very important to me and I wanted to translate that into this project. I concluded that a Workout program app which kept track of a user's daily workout program would meet the requirements.

The first thing I did before I started my project was to visualize what types of models, views, and controllers I needed. From there I was able to set up a basic skeletal structure and add  my database migrations. With this initial part of the project set up, I was able to get a working base.

On a side note, I found that the Corneal gem would have helped me install a basic skeletal structure automatically. Unfortunately, I only found out about this gem after I got set up. I would highly recommend anyone reading this to start off by installing the Corneal gem. 

In terms of filling my MVC structure, I started off by filling out my models which includes Exercises, User, and Helper. The reason why there is a Helper model is simply because I prefer it that way.

After the models were filled out, I made sure that my signup and login routes in my user controller were working with the assigned views. In my opinion, it was much easier for me to figure out the user controller first.

From there, I worked through CRUD with my exercises controller by concurrently tweaking my controllers and views until it worked. A big contributor to completing this portion was my successful completion of the Fwitter group project. This previous project helped soldify some concepts and made Sinatra come together in my eyes.

It wasn't all smooth sailing from there, the biggest challenges I encountered were assigning individual exercises to their associated accounts and ensuring that users couldn't modify content created by other users.

Once I overcame these hurdles, I inserted user input validations and error messages in the form of flash messages. In addition, I linked my views together in order to create a more user friendly interface.

Conclusion

As with any student learning programming/web development for the first time, I particularly faced a lot of self doubt over the past few weeks over learning Sinatra. With the completion of this project, I am feeling quite accomplished and proud about what I have done.

Although I'm proud of my achievement, I know that my code is not perfect. I'm looking forward to refactoring my code and learning more about best practices for a working Sinatra app.

