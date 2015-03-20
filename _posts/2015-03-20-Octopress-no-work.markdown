---
layout: post
title: Octopress no work 
---
Well, I guess Octopress 3.0 doesn't seem ready for primetime. I kept getting this error that a couple people seemed to be getting fairly often:

{% highlight %}
$ octopress new post "test post"
octopress 3.0.0.rc.34 | Error:  undefined method `require_from_bundler' for Jekyll::PluginManager:Class
{% endhighlight %}

Here[https://github.com/octopress/octopress/issues/94] and here[https://github.com/mmistakes/skinny-bones-jekyll/issues/22] are two different places where I found some problems.
