---
layout: post
comments: false
title: A case for the bioinformatics manifesto
---

Software development is complex and as you would expect there are [several software development approaches](http://www.quora.com/What-is-are-the-best-software-development-philosophy-ies), philosophies and principles. Most organisations ascribe to one or more of these approaches. The Agile and the Unix philosophies are widely adopted in most organisations and by individuals.

The [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy) advocates for programs that do one thing very well. Programs that work together and provide universal interfaces and in particular to text streams. The idea stems from years of experience developing the Unix tools. The Unix philosophy it is not a written manifesto that you have to ascribe to or sign, it is a respected tradition that organically grew from writing the early Unix operating system and associated tools.

The [Agile manifesto](https://en.wikipedia.org/wiki/Agile_software_development) aims at delivering working software. It emphasizes on continuous testing and deployment, places special emphasize on working with the client, consulting regularly and lack of formal cast-in-stone methods. It is not surprising that agile initially appeared as anti-establishment, disruptive approach to formal software development methods. Agile process was quick to be adopted by early disruptive technologies like Ruby on Rails and their architects came to be Agile’s staunchest evangelists.

With maturation as a scientific discipline, a pride in Unix and Linux tradition with a rich client base of biologists, you would be mistaken to think that most bioinformatics tools would embrace the Unix philosophy and apply the Agile process. Instead, bioinformatics software is a thorny garden. The field is comparable to a half sinking ship that magically remains afloat and somehow manages to deliver cargo. Often the passengers take the wheel for an adrenaline serge with undesirable consequences.

I think this is what has led to the current efforts to establish a bioinformatics software philosophy and written manifesto, the bioinformatics manifesto aka [small tools for bioinformatics](https://github.com/pjotrp/bioinformatics). It begins by stating that bioinformatics tools are fragmented largely due to the key challenges with biological data and analysis which include: scaling of calculations, full data integration, interaction and visualization
The manifesto also aims at countering current trends where "institutes and companies create monolithic software solutions for end users". These tools are often exceedingly expensive and not interoperable with other tools in the same domain. It is a call to the Unix philosophy and practice 
and the use of transparent open source licenses.

The manifesto goes a step further to address how to package and distribute bioinformatics tools. The current bioinformatics software packaging 
system is broken. A URL is as good as the acceptance of the publication describing the tool(s). Thereafter, the tool is not maintained and even better,
it disappears with total disregard to the current and potential users. Releases can be far between and collaboration is  non-existent.

So will small tools for bioinformatics deliver? That remains to be seen. But first it has to gain a wide adoption and acceptance. As of this writing,
48 bioinformaticians have [publicly signed the manifesto](https://github.com/pjotrp/bioinformatics). 
It is a rational approach to start weeding and pruning the thorny garden of bioinformatics software. It does not advocate for new fangled ideas or philosophy, it is a call to remain true to tested approaches in software development.

{% include twitter_plug.html %}
