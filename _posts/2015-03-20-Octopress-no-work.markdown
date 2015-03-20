---
layout: post
title: Octopress no work 
date: 2015-03-20 02:20:00 -0600
---
Well, I guess Octopress 3.0 doesn't seem ready for primetime. I kept getting this error that a couple people seemed to be getting fairly often:


	$ octopress new post "test post"
	octopress 3.0.0.rc.34 | Error:  undefined method `require_from_bundler' for Jekyll::PluginManager:Class


[Here](https://github.com/octopress/octopress/issues/94) and [here](https://github.com/mmistakes/skinny-bones-jekyll/issues/22) are two different places where I found those same problems. I think I'm going to go ahead and forego Octopress for just using Jekyll all by itself. I suppose I can write date/time into posts and YAML...
