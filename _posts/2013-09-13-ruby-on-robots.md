---
layout: post
title:  "Ruby on Robots"
date:   2013-09-13 11:47:13
categories: ruby, robots
---

While the majority of ruby development is tied to Rails and other web frameworks, but ruby is a very powerful scripting language that other sectors have found some excellent uses for.

Enter [Artoo](http://artoo.io/). Artoo is a fantastic project that aims to show how pleasant ruby can be to write.

It aims to have hooks in [AR Drones](http://ardrone2.parrot.com/), [Arduino](http://www.arduino.cc/), [Roomba](http://www.irobot.com/us/learn/home/roomba.aspx), [Pebble](http://getpebble.com/), [Leapmotion](https://www.leapmotion.com/), and many others. In this case, you can make a [Sphero](https://www.gosphero.com/) dance like an idiot:

```ruby
work do
  every(3.seconds) do
    puts "Rolling..."
    sphero.roll 60, rand(360)
  end
end
```

Artoo relies heavily on [Rubinius](http://rubini.us/) for their translation, which is what allows them to optimize their code so well for embedded systems.

[Check out Artoo in Action!](http://artoo.io/videos/)