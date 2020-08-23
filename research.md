---
layout: page
permalink: /research/
title: Research
pubs:

    - title:   "The Impact of CEO Pay and its Disclosure on Stock Price Crash Risk: Evidence from China"
      author:  "Jiahua Xu, Lan Zou"
      journal: "China Finance Review International"
      number:    "9(4):479-497"
      year:    "2019"
      url:     "https://doi.org/10.1108/CFRI-10-2018-0138"
      
wps:

    - title:   "Explaining Consumer Choice in Health Insurance: The Role of Prevalent Normative and Descriptive Models"
      author:  "Lan Zou"
      abstract: "This paper describes"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2014"
      url:     " "
      doi:     "http://dx.doi.org"
      image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"

    - title:   "The Welfare Effect of Poor Decisions in Health Insurance"
      author:  "Christian Biener, Lan Zou"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2014"
      url:     " "
      doi:     "http://dx.doi.org"
      image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"

    - title:   "The Value of Choice"
      author:  "Christian Biener, Lan Zou"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2013"
      url:     " "
      doi:     "http://dx.doi.org"
      image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"

    - title:   "Health Insurance Risk Premium:Finding the Right Price"
      author:  "Lan Zou"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2013"
      url:     " "
      doi:     "http://dx.doi.org"
      image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"

---



## Working Papers

{% for item in page.wps %}
{% if item.url %}[**{{item.title}}**]({{item.url}}){:target="_blank"}{% else %}**{{item.title}}**{% endif %}<br />
{{item.author}}
{% endfor %}

## Publications 

{% assign thumbnail="left" %}

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}