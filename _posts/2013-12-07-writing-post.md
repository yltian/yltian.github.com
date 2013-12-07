---
layout: post
title: "writing post"
categories:
- 
tags: jekyll writing posts
- 


---

Writing posts
===============

The Posts Folder
-------------------

As explained on the [directory structure] page, the `_posts` folder is where
your blog posts will live.These files can be either [Mardown] or [Textile]
formatted text files, and as long as they have [YAML front-matter], they will
be coverted from their source format into an HTML page that is part of your
static site.

Creating Post Files
-------------------

To create a new post, all you need to do is create a new file in the `_posts`
directory. How you name files in this folder is important. Jekyll requires blog
post files to be named according to the following format:

> YEAR-MONTH-DAY-title.MARKUP

For example, the following are examples of valid post filenames:

{% highlight bush %}
2011-12-04-new-years-eve-is-awesome.md
{% endhighlight %}

Including images and resources
----------------------

Because of Jekyll's flexibility, there are many solutions to how to do this.
One common solution is to create a folder in the root of project directory
called something like `assets` or `downloads`, into which any image, downloads
or other resources are placed. Then, from within any post, they can be linked
to using the site's root as the path for the asset to include. Again, this will
depend on the way your site's (sub)domain and path are configured, but here
some examples (in Markdown) of how you could do this using the `site.url`
variable in a post.

{% highlight text avrasm %}
... which is shown in the screenshot below:
![My helpful screenshot]({{ site.url }}/assets/screenshot.jpg)
{% endhighlight %}

{% highlight text avrasm %}
... you can [get the PDF]({{ site.url }}/assets/mydoc.pdf)
{% endhighlight %}

Higlighting code snippets
-----------------------

{% highlight ruby %}
def show
    @widget = Widget(params[:id])
    respond_to do |format|
        format.html #show.html.erb
        format.json { render json: @widget }
    end
end
{% endhighlight %}


-- EOF --
