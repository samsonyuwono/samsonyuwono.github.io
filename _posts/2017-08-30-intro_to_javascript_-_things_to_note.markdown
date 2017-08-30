---
layout: post
title:  "Intro to Javascript - Things to note"
date:   2017-08-30 11:04:14 -0400
---

After coding and writing applications in Ruby for 3 months, the Flatiron School syllabus has finally brought me back into Javascript.

Now that I'm reviewing my first programming language. I wanted to provide the Learn community with a few tidbits and notes on a few syntactic differences between Javascript and Ruby.

One of the biggest syntactic differences I noticed in my transition back to JS was the emphasis on defining every variable.

For example in Ruby a variable would typically be defined like this: 

`variable_name = variable_value` vs `var variable_name = variable_value`
These lines are essentially the same but JS requires a `var` to set every variable.

Functions vs. Methods
Functions in JS is equivalent to methods in Ruby. The differences are demonstrated in the images below.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/HmXeI"><a href="//imgur.com/HmXeI"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>


<blockquote class="imgur-embed-pub" lang="en" data-id="a/flpi3"><a href="//imgur.com/flpi3"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

`== vs ====`

In ruby the double equals sign is used for equality in conditional statements like an if statement.

Although at first glance the difference between `==` and` ===` in JS can be negligible. The truth is `==` doesn't bother with types. 

For example:  `(1== "1")` returns true 

`(1 === "1")` returns false. 

The second example returns false because the comparison is between a number and a string. Therefore, if the second value was a number, the statement would return true. In a nutshell, the triple equals sign will return true if the two objects were the same typeof and value.

typeof vs .class
When I referred to typeof in the last paragraph I am referring to how JS determines the value of something. The values including but not limited to number, string, or an array.  In Ruby, .class is the equivalent of typeof. The images below outline the similarities.

<blockquote class="imgur-embed-pub" lang="en" data-id="a/qt81e"><a href="//imgur.com/qt81e"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

<blockquote class="imgur-embed-pub" lang="en" data-id="a/MLKr1"><a href="//imgur.com/MLKr1"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>






