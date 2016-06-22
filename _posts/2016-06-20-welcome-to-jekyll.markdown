---
layout: post
title:  "Create website with jekyll and serve on github!"
date:   2016-06-20 17:29:43 +0300
categories: jekyll update
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

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

```java
public DashboardFuelInfoResponseDto getFuelInfo(Integer argUserId, Character argType, Integer argId, DateRangeDto argDateRange)
	{
		DashboardFuelInfoResponseDto fuelInfo = null;
		List<Object> parameterList = new ArrayList<Object>();
		parameterList.add(argUserId);
		parameterList.add(argType);
		parameterList.add(argId);
		parameterList.add(argDateRange.getStart());
		parameterList.add(argDateRange.getEnd());
		try
		{
			fuelInfo = DatabaseUtil.callReadOnlyStoredProcedure(this.dataSource, StoredProcedureEnum.s_getDashboardFuelInfo, parameterList, new DashboardFuelInfoExtractor());

		} catch (SQLException e)
		{
			throw new DAOException(e.getMessage(), e);
		}

		return fuelInfo;
	}
```

{% highlight java %}
@RequestMapping(value = "/settings/updateidlefuelconsumption", method = RequestMethod.POST)
@ResponseBody
public Object updateIdleFuelConsupmtion(NgUserDto argNgUserDto, @RequestBody @Valid FloatParamDto argFloatParam)
{
	return this.companyService.updateIdleFuelConsupmtion(argNgUserDto.getUserCompanyId(), argFloatParam.getFloatParam());
}
{% endhighlight %}

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this ~~post~~ to get an idea about how it works.

@pherdee

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

{% highlight json %}
{
"success":true,
"type":"SUCCESS",
"message":null,
"result":
}
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

Inline-style:
![alt text](http://ferdisonmezay.com/2015/images/0.jpg "Logo Title Text 1")

Reference-style:
![alt text][logo]

[logo]:http://ferdisonmezay.com/2015/images/0.jpg "Logo Title Text 2"

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
