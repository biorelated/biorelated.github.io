---
layout: post
comments: false
title: Publication quality plots with cowplot
---

I often turn to [ggplot2](http://docs.ggplot2.org/current/) for creating statistical plots.
(Read Hadley's excellent tutorial on [how to build a plot with ggplot2](https://rpubs.com/hadley/ggplot2-layers)). 
Ggplot2 is an implementation of the [grammar of graphics](http://www.tandfonline.com/doi/abs/10.1198/jcgs.2009.07098),
a concise approach for describing the components of a graphic.

It often takes extra effort to arrange ggplot2 objects on a grid. On many occasions,  the code looks like a hack.
In addition, R does not offer very clean syntax and therefore the code can be difficult to read and understand.
Here is a snippet of code that I was using to print four ggplot2 objects on a 2 x 2 grid.

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

With cowplot I can reduce the seven lines of code to just a single line one! This may not seem a lot, but for the sake
of brevity, beauty and intent, I think it is a big deal.

{% highlight r %}
  
  plot_grid(plot1,plot2,plot3,plot4,labels=c("A","B","C","D"),nrow=2)

{% endhighlight %}

The above code is more legible than the previous code. The code also places labels to each plot, which 
is a winner feature for publication quality graphics. Many journals and reviewers expect well labelled graphics.
Cowplot offers many excellent defaults and it can [do a tonne more](http://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html).

{% include twitter_plug.html %}
