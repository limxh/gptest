## Welcome to Maple Publish

## Article Title
| Date :"`r format(Sys.time(), '%d %B, %Y')`"        | Authors: John Doe    | <Contact@example.com>       |date: "`r Sys.Date()`"|

___
{% highlight ruby %}
{{ site.time | date_to_long_string: "ordinal" }}
{% endhighlight %}

{{ site.time | date_to_long_string: "ordinal" }}

{{ article.published_at | date: "%a, %b %d, %y" }}

# 1. Can GitHub Pages host HTML

# 2. Can we customise our md theme in Github Pages

https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll

# 3. Ways to let GitHub Pages support non static site

# 4. Jekyll Gallery Generator

https://github.com/ggreer/jekyll-gallery-generator

# 5.Useful plugins

> We can enable additional plugins by adding the plugin's gem to the plugins setting in your _config.yml file. For more information, see "Configuration" in the Jekyll documentation.

https://github.com/topics/jekyll-plugin
https://github.com/planetjekyll/awesome-jekyll-plugins


This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.



[Home Page](../../index.md)
<div style="text-align: right"><a href="../../index.md" >Next Chapter</a> </div>