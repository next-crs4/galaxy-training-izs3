---
layout: default
title: Home
---

<a href="https://www.crs4.it/" target="_blank"><img src="{{site.url}}/images/CRS4-logo.png" width="200"></a>
## [{{site.title}}]({{site.url}})

---

{::nomarkdown}

{% assign pages_list = site.pages | sort:"url" %}
    {% for node in pages_list %}
      {% if node.title != null %}
        {% if node.layout == "page"  and node.hide == null %}
          <a class="sidebar-nav-item{% if page.url == node.url %} active{% endif %}" href="{{site.url}}{{ node.url }}">{{ node.title }}
          <p class="note">{{node.summary}}</p></a>
        {% endif %}
      {% endif %}
    {% endfor %}
{:/}

--- 

### Authors and Contributors

 * [Rossano Atzeni](http://www.crs4.it/peopledetails/357/rossano-atzeni)
 * [BIOSCIENCES AND COMPUTATIONAL INFRASTRUCTURES, SMART PROJECTS AND QUANTUM COMPUTING](https://www.crs4.it/research/bcqc/)

<table style="border:1px solid white;">
<tr>
<td style="background-color:white; border:1px solid white;">
<br>
<a href="https://next.crs4.it/" target="_blank"><img src="{{site.url}}/images/CRS4-NEXT-logo.png" width="300"></a>
</td>
<td style="background-color:white; border:1px solid white;">
<a href="https://next.crs4.it/" target="_blank"><img src="{{site.url}}/images/CRS4-HPC-logo.png" width="300"></a>
</td>
</tr>
</table>

Some of the materials used in this training are from the 
[Galaxy community](https://github.com/galaxyproject/training-material) and are the result of a collaborative work. 
Thanks to [all the contributors](https://github.com/galaxyproject/training-material/graphs/contributors) 
and the Galaxy Training Network!

![]({{site.url}}/images/GTN.png)