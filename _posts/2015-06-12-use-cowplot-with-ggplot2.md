---
layout: post
comments: false
title: Publication quality plots with cowplot
---

I often turn to [ggplot2](http://docs.ggplot2.org/current/) for creating statistical plots. (See this tutorial on [how to build a plot with ggplot2](https://rpubs.com/hadley/ggplot2-layers)).
It is an amazing plotting library based on the grammar of graphic concept. 

It often takes extra effort to arrange ggplot2 objects into a grid. Often the code feels like a hack.
In addition, R does not offer clean syntax. Therefore code can be difficult to read and understand. 
Here is a snippet of code that I was using to display 4 plots in a 2x2 grid,

{% highlight r %}
  #new grid
  grid.newpage()
  
  #a 2 rows and 2 columns viewpoint
  pushViewport(viewport(layout = grid.layout(2,2)))

  #a function to render each viewpoint
  vplayout <- function(x, y) viewport(layout.pos.row = x, layout.pos.col = y)

  #print each plot in its respective area/grid
  print(plot1, vp = vplayout(1, 1))
  print(plot2, vp = vplayout(1, 2))
  print(plot3, vp = vplayout(2, 1))
  print(plot4, vp = vplayout(2, 2))

{% endhighlight %}

and now with cowplot I can simply turnoff the verbosity and get a one-liner! 

{% highlight r %}
  
  plot_grid(plot1,plot2,plot3,plot4,labels=c("A","B","C","D"),nrow=2)

{% endhighlight %}

That is much better and more legible than the previous code. The labels are really the key publication property that
is easy to do with cowplot. Most journals expect a neat and well labelled graphic. The default ggplot2 parameters do not 
allow producing such plots. 

Cowplot offers excellent defaults and it can [do a lot more than this](http://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html).

{% include twitter_plug.html %}
