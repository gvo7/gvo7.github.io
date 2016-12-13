---
layout: post
title:  "Building a Phoenix Web Application from scratch"
date:   2016-12-13 18:00:01 +0200
categories: elexir phoenix
---

Creating a new project

{% highlight elexir %}
mix phoenix.new newproject
{% endhighlight %}

After all dependencies are installed.

{% highlight elexir %}
cd newproject
mix ecto.create
mix phoenix.server
{% endhighlight %}
