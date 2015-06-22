---
layout: post
title:  "Welcome to Jekyll!"
date:   2014-11-08 11:13:26
categories: jekyll update
---
Write stuff here--in (kramdown) markdown

Code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Drafts are posts without a date in _drafts. To preview your site with drafts, simply run jekyll serve with --drafts

Where you put HTML files for pages depends on how you want the pages to work. There are two main ways of creating pages:
Place named HTML files for each page in your site’s root folder.
Create a folder in the site’s root for each page, and place an index.html file in each page folder.
Both methods work fine (and can be used in conjunction with each other), with the only real difference being the resulting URLs.

Use the post_url tag to link to other posts without having to worry about the URL's breaking when the site permalink style changes.

For images...
… which is shown in the screenshot below:
![My helpful screenshot]({{ site.url }}/assets/screenshot.jpg)
Or PDF linking...
… you can [get the PDF]({{ site.url }}/assets/mydoc.pdf) directly.

You can skip the {{ site.url }} variable if you know your site will only ever be displayed at the root URL of your domain. In this case you can reference assets directly with just /path/file.jpg.

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].