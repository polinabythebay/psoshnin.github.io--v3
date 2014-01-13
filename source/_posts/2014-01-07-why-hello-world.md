---
layout: post
title: "Why hello world"
tagline: "Supporting tagline"
description: "this is a description"
category: acatetory
tags: [thisisatag]
---
{% include JB/setup %}

Here is a ruby snippet, it's kinda cute:

{% highlight ruby linenos%}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}
