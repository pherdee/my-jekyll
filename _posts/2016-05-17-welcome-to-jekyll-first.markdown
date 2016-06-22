---
layout: post
title:  "Welcome to Jekyll - First!"
date:   2016-05-17 14:51:20 +0300
categories: jekyll update
backcolor: f0c301
---

On github :

create a repository : my-jekyll

create `gh-pages` branch

on local:

clone repository `git clone`

change branch `git checkout gh-pages`

create jekyll website `jekyll new`

change configuration baseurl : `my-jekyll`

run `jekyll build`


run `git add *`

run `git commit -m "first jekyll"`

run `git push`

go to `https://pherdee.github.io/my-jekyll/`

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
@RequestMapping(value = "/insert", method = RequestMethod.POST)
@ResponseBody
public Object insertDriver(NgUserDto argNgUserDto, @RequestBody @Valid MuDriverRequestDto argDriver)
{
	argDriver.setCompanyId(argNgUserDto.getUserCompanyId());
	this.driverService.isDallasCodeValid(argNgUserDto, argDriver);
	this.driverService.insertDriverAndAssignVehicle(argNgUserDto, argDriver);
	return Boolean.TRUE;
}
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
