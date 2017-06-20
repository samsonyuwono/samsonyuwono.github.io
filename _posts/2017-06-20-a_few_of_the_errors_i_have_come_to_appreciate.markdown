---
layout: post
title:  "A few of the errors I have come to appreciate"
date:   2017-06-20 14:09:32 +0000
---



As anyone who has gone through schooling, we are conditioned to avoid errors and red marks. Although I still hate seeing errors, I have come to appreciate their usefulness when it comes to programming. 

In order to help new students in this course, I will outline a few common errors below to explain what the error is and where to exactly to look to fix it. .



Syntax Error
This one is pretty simple to figure out but gets confusing when you don't know what to find what you're looking for. Typically the error message tells where exactly to look it. In the case where you still can't fix the syntax error, I highly recommend googling the method syntax to get an idea of what you're doing doing incorrectly.

Argument Error
This one is pretty simple and straightforward. It's raised when the amount of errors are wrong or when you're passing an argument that is unacceptable. My recommendation to overcome this error is to understand exactly what your method is taking in.

NoMethod Error
This error is raised when a method is called on a receiver that doesn't have it defined.  In this case, a receiver is a Ruby object whose method is being invoked. The opposite is true for a sender, where an object is invoking a method. 

Name Error
This error is raised when a name is invalid or undefined. Check to see which of your method variables are not being defined. NameErrors might read like the following.

`NameError: undefined local variable or method foo for main:Object
NameError: wrong constant name answer`


When I was new to coding, I didn't understand what to do or how to approach these errors, so my intention with this blog post is to alleviate the concerns of newer students to the Flatiron Web Development Immersive. 

