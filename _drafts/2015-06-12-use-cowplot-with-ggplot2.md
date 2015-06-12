---
layout: post
comments: false
title: Use cowplot with ggplot2
---

There is nothing like finding that technical thing you have been wanting to implement and then it appears right in your eyes
just like magic. Well not exactly, but you know what I mean. I use ggplot2 extensively for all my plots. 
It is an amazing library but sometimes to get exactly what you want, sometimes you have to hack it, coupled with R's horrible syntax you come up with a horrible hack but beautiful plot.

Here is a snippet of code that I was using to display 4 plots in a grid,
{% highlight r %}
  
  grid.newpage()
  pushViewport(viewport(layout = grid.layout(2,2)))
  vplayout <- function(x, y) viewport(layout.pos.row = x, layout.pos.col = y)

  print(plot1, vp = vplayout(1, 1))
  print(plot2, vp = vplayout(1, 2))
  print(plot3, vp = vplayout(2, 1))
  print(plot4, vp = vplayout(2, 2))

{% endhighlight %}

and now with cowplot I can simply turnoff the verbosity. 

{% highlight r %}

  plot_grid(plot1,plot2,plot3,plot4,labels=c("A","B","C","D"),nrow=2)

{% endhighlight %}

That is much better and more legible than the previous code to achieve the same effect.


