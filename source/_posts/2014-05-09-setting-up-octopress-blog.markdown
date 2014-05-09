---
layout: post
title: "Setting up Octopress Blog"
date: 2014-05-09 23:24:37 +0530
comments: true
categories: Blogging Jekyll Octopress
---

So, I finally begin to blog again! All thanks to a blogging framework crashed into accidentally, of course.

[Jekyll.rb](http://jekyllrb.com/) is one powerful micro-blogging framework written in Ruby. It comes with a unique integrator that can easily create, segment and categorize blog posts without hassles. You simply create apost, edit/change, publish and your post is ready. Right in your own site.

Github is advantageous in a lot of ways - social coding, side projects, open source and cool hacks. It now bumpered with a bonanza - [The GitHub Pages](https://pages.github.com/). WHat I finally found from the boring wordpress is that, it can be configured, the way we want, the style we like and the site we wish(although, with a site-domain purchase).

Finally, the combination of above turned out to be [Octopress](http://octopress.org/). This is one of the most easiest blog engines, a programmer can fall in love with. Of course, keeping in mind the love of programming but blogging simultaneously. We as programmers tend to do stuff by code all the time and this came as a convenience. What's more is that you can show off keeping your skills intact.

Such engines help in a lot of ways of learning -

	1. A programming language - Ruby.
	2. A template engine.
	3. Automating posts - the markdown
	4. versioning for site and source - git

Good that if I'm just scribbling, I'm not just writing stuff up. I'm programming too. So, let me begin the new, old journey of blogging back into the life - with a way I always wanted. 

I wanted to add some lines to how to setup your own blog via Octopress too.

* Get yourself a GitHub user, please. You won't regret.
* Setup your site via [GitHub Site Hosting](https://pages.github.com/)
* Install the [Octopress-Jekyll](http://octopress.org/docs/setup/) bundle.
* Make sure you [deploy your site properly](http://octopress.org/docs/deploying/github/)
* Start Blogging!

Now for the missing part. Octopress provides you a clean way of setting up. However, there are some glitches during continuous blogging - Git might give problems or something will break down so here's my extra findings:

* When you write/edit posts, first commit the changes
* Generate the site using `bundle exec rake generate` and deploy to `master` branch via `bundle exec rake deploy`. This will first add the site.
* Push source branch to your repo too (`git push origin source`). This will ensure you can work anywhere you want with a simple pull/clone. 

Enjoy!
