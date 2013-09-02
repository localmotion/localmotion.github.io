---
layout: post
title:  "Reasons to love Ruby"
date:   2013-09-02 11:47:13
categories: ruby
---

The other day I was trying to get the data of a day 50 days ago using JavaScript. As often happens when I am working with JavaScript, I remember how much I love the fact that I mostly write in Ruby.

Ruby:

````ruby
50.days.ago
````

vs Javascript

````javascript
new Date(new Date().setDate(new Date().getDate()-50))
````

You can see why I would prefer the ruby way. Here are couple other examples.

Python:

````python
from datetime import date, timedelta
d=date.today()-timedelta(days=days_to_subtract)
````

And trusty Java:

````java
Date d = initDate();
Date dateBefore = new Date(d.getTime() - 50 * 24 * 3600 * 1000 );  
````