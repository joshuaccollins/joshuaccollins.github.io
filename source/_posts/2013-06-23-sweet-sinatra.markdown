---
layout: post
title: "Sweet Sinatra"
date: 2013-06-23 11:35
comments: true
categories: 
---

SinMagick a front-end for image processing and thumbnailing with flexible storage options.


## Rapid Dashboard Making with Dashing

![Large icon](http://shopify.github.io/dashing/images/bowtie.png ")

Using the one and only Ruby Sinatra developers are able to create high resolution dashboards using [Dashing.](http://shopify.github.io/dashing/) This framework was originally created by the developers at Shopify who wanted to display custom dashboards on TV's around the office showing their progress and success. Since Shopify is an epicly awesome company I decided to take a closer look under the hood to see what we could find.

####Main takaways:

- Use premade widgets, or fully create your own with scss, html, and coffeescript.

- Widgets harness the power of data bindings to keep things DRY and simple. Powered by batman.js.

- Use the API to push data to your dashboards, or make use of a simple ruby DSL for fetching data.

- Drag & Drop interface for re-arranging your widgets.

- Host your dashboards on Heroku in less than 30 seconds.

- Every new Dashing project comes with sample widgets & sample dashboards for you to explore. 

- Widgets use [batman bindings](http://batmanjs.org/docs/batman.html#batman-view-bindings-how-to-use-bindings) in order to update their contents. Whenever the data changes, the DOM will automatically reflect the changes.

- When you pass in data with a title attribute, the widget's title variable will change, and so will all DOM elements bound to it. No need to handle that yourself which is nice.

#### A responce from Shopify on the following question:

"Why use Dashing when there are plenty of cloud based dashboards out there?"

###### Use our own authentication. 
  Many online platforms give you private URLs to your dashboards. Those can be tricky to remember, and can accidentally fall in the wrong hands. With Dashing, you can add whatever auth you want. We use Google Auth.

##### Be completely customizable. 
  We didn't want to be limited by the widgets that are available on other platforms. We also wanted all of our code to be in version control, and editable in whatever IDE we want.

##### Keep instances of the same widget in sync. 
  Many online dashboards give unique ids for every widget instance you create. This means that if you want to update 3 identical widgets showing 'daily sales', you'll need to use the API to push the value to all 3 instances. With Dashing, identical widgets all have the same id, meaning less duplication, and complete synchrony across all dashboards.


That's it for my review of Dashing. Looks like a pretty cool tool for dashboards. Just remember I'm only four weeks into my development careers so take everything with a grain of salt. Main information from this post comes from [Shopify's Github portal](http://shopify.github.io/dashing/) & [wiki](https://github.com/Shopify/dashing/wiki).

##### Bonus: [Click here to checkout some live dashboard build on Dashing!](http://dashingdemo.herokuapp.com/sample)

[Feedback is always welcome. Drop me a line!](https://twitter.com/jcalebCollins)

###### Onward!