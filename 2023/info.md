### Table of Contents

{%- assign top_ten_pages = site.pages | where:"document","OWASP Machine Learning Security Top Ten 2023" | sort: "order" %}
<ul>
{%- for ttp in top_ten_pages -%}
{%- unless ttp.order == 0 %}
<li><a href="{{site.baseurl}}{{ ttp.url }}">{{ ttp.title }}</a></li>
{%- endunless -%}
{% endfor %}
</ul>
