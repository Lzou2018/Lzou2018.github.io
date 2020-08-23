---
layout: page
title: CV
permalink: /cv/
acajobs:

    - title:    "Research Project Manager"
      org:      "University of St.Gallen"
      orgurl:   "https://www.ivw.unisg.ch/"
      country:  "Switzerland"
      start:    "04/2018"
      end:      "present"

     
education:   
    - title:    "Project Manager and Research Associate"
      org:      "Institute of Insurance Economics, University of St.Gallen"
      orgurl:   "https://www.ivw.unisg.ch/"
      country:  "Switzerland"
      advisor:  "PD. Dr. Christian Biener"
      advurl:   "https://sites.google.com/site/bienerresearchprofile/"
      start:    "06/2018"
      end:      "present"       
    - title:    "M.Sc. in Financial Management"
      org:      "Area Banking, Finance & Insurance, Business School, University of Birmingham"
      orgurl:   "https://www.birmingham.ac.uk/index.aspx"
      country:  "UK"
      start:    "08/2017"
      end:      "06/2018"
    - title:    "BBA in Accounting"
      org:      "Accounting, Beijing Business and Technology University,China"
      orgurl:   "http://english.btbu.edu.cn/"
      country:  "China"
      start:    "07/2009"
      end:      "07/2013"
      indjobs:

indjobs:
    - title:    "Manager in Risk Management Department"
      org:      "Nanning Juxing Micro-Credit Co., Ltd,Guangxi Communications Investment Group Co., Ltd, China"
      orgurl:   "http://www.gxjttzjt.com/"
      country:  "China"
      start:    "04/2014"
      end:      "07/2016"
    
    - title:    "Accountant"
      org:      "ShenZhen Haiya Group Co., Ltd, China"
      orgurl:   "http://www.hygroup.cc/index.html"
      country:  "Shenzhen,China"
      start:    "09/2012"
      end:      "02/2013"
    
    - title:    "Intern in Accounting"
      org:      "Sony(China) Co., Ltd., China"
      orgurl:   "https://www.sony.com.cn/"
      country:  "Beijing,China"
      start:    "10/2013"
      end:      "03/2014"

---

## Research and Academic Positions

<!-- {% assign thumbnail="left" %} -->

{% for item in page.acajobs %}
*{{item.start}} --- {{item.end}}*
<br />
**{{item.title}}**
<br />
[{{item.org}}]({{item.orgurl}}){:target="_blank"}, {{item.country}}
{% endfor %}

## Educational Experience

{% for item in page.education %}
*{{item.start}} --- {{item.end}}*
<br />
**{{item.title}}**
<br />
[{{item.org}}]({{item.orgurl}}){:target="_blank"}, {{item.country}}{% if item.advisor %}
<br />
Advisor: [{{item.advisor}}]({{item.advurl}}){:target="_blank"}
{% endif %}
{% endfor %}

## Industry Experience

<!-- {% assign thumbnail="left" %} -->

{% for item in page.indjobs %}
*{{item.start}} --- {{item.end}}*
<br />
**{{item.title}}**
<br />
[{{item.org}}]({{item.orgurl}}){:target="_blank"}, {{item.country}}
{% endfor %}

Download [Full version](https://www.dropbox.com/s/57hi9guvrhth1di/Lan_Zou_CV_20190919.pdf?dl=0). 


