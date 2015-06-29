---
layout: post
comments: false
title: A case for a bioinformatics manifesto
---

Software development can be a complex process and therefore [several software development approaches](http://www.quora.com/What-is-are-the-best-software-development-philosophy-ies), philosophies and principles have emerged. Many organisations ascribe to one or more of these approaches depending on the size of the development team and the nature of the problem or task. The Agile and the Unix philosophies have come to be widely adopted in most organisations and also by individual developers.

The [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy) advocates for programs that do one thing very well. Programs that work together and provide universal interfaces and in particular to text streams. The idea stems from years of experience developing the Unix tools. The Unix philosophy it is not a written manifesto that you have to ascribe to or sign, it is a respected tradition that organically grew from writing the early Unix operating system and associated tools.

The [Agile manifesto](https://en.wikipedia.org/wiki/Agile_software_development) aims at delivering working software. It emphasizes on continuous testing and deployment, places special emphasize on working with the client, consulting regularly and lack of formal cast-in-stone methods. It is not surprising that agile initially appeared as anti-establishment, disruptive approach to formal software development methods. Agile process was quick to be adopted by early disruptive technologies like Ruby on Rails and their architects came to be Agile’s staunchest evangelists.

With maturation as a scientific discipline, a pride in Unix and Linux tradition with a rich client base of biologists, you would be mistaken to think that most bioinformatics tools would embrace the Unix philosophy and apply the Agile process. Instead, the bioinformatics software field is often a thorny garden. The field is comparable to a half sinking ship that magically remains afloat and somehow manages to deliver cargo. Often the passengers take the wheel for an adrenaline serge with undesirable consequences.

An attempt to overcome the current challenges has led to establishment of a [bioinformatics software manifesto](https://github.com/pjotrp/bioinformatics). According to this manifesto, bioinformatics tools are fragmented due to challenges in integration, interaction and visualization of biological data as well as scaling of calculations. It emphasizes on developing what it calls "small tools for bioinformatics".

The manifesto challenges and criticizes the current trends where "institutes and companies create monolithic software solutions for end users". These tools are often exceedingly expensive and not interoperable with other tools that are within the same domain. It calls for the adoption of the unix philosophy and the use of transparent open source licenses in bioinformatics.

Bioinformatics software packaging system is broken and fragmented as well. A web resource is disregarded as soon as an 
article is accepted in a journal. Where a tool exists, releases can be far between and collaboration is difficult or non-existent. The worst cases is where tools are developed without making use of a revision control mechanism. Small tools for bioinformatics calls for a standard approach to bioinformatics software packaging and distribution. 

So will small tools for bioinformatics deliver? That remains to be seen. But first it has to gain a wide adoption and acceptance. As of this writing,
48 bioinformaticians have [publicly signed the manifesto](https://github.com/pjotrp/bioinformatics). 
It sounds like a rational approach to start weeding and pruning the thorny garden of bioinformatics software.

{% include twitter_plug.html %}
