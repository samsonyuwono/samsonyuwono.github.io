---
layout: post
title:      "How does the Fetch API work"
date:       2017-12-28 16:48:50 +0000
permalink:  how_does_the_fetch_api_work
---


In the past, in order to get data of an API, you would have had to use XMLHttpRequest. The Fetch API allows you to make network requests similar to XMLHttpRequest but in a more streamlined process. This streamlined process is due to the fact that Fetch sends all requests in one initial asynchronous task that returns a Promise object. Whereas XMLHttpRequest sends requests to a server in a synchronous manner (back and forth).

On a high level, the reason why the Fetch API enables this efficiency is because it uses Promises. In JavaScript, a Promise is an object that represents a value that may not be available yet but will be resolved at some point in the future. In the context of the Fetch API, the promise is an object that represents the result of an operation when it occurs. 

Fetch also implements a powerful feature of thenable called `then()`. We can chain each then() call to receive the result of the previous argument. 

```    fetch(`http://localhost:3001/api/players`)
    .then(response => response.json())
    .then(players => console.log(players))
```

In the code above, fetch is making a request to the api containing an array of object containing players. The line `.then(response => response.json())` is getting the response from fetch using the `.json` method to turn it into JSON. The last line then takes the response a console.log the results.

Calling `response.json()` in the fetch is a simple way of getting the response parsed as JSON. This is because the fetch API includes Body, which has functions that specialize in transforming the body of a request or response. More info on Body is in the link below.

**https://developer.mozilla.org/en-US/docs/Web/API/Body**

Then it’s passing the JSON to the next line to be handled by the following function `.then(players => console.log(players))`. 

The result is the display of the JSON object in the console. 

<blockquote class="imgur-embed-pub" lang="en" data-id="a/XLYfr"><a href="//imgur.com/XLYfr"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

