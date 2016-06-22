---
layout: post
title:  "Hoşgeldiniz"
date:   2016-05-17 18:51:20 +0300
categories: jekyll update
backcolor: 8D3C60
fontcolor: af5f90
---


-

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

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
