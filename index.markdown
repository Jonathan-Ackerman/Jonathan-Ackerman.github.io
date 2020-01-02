---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<h2>Projects</h2>
<ul>
{% assign sorted = site.projects | sort: 'dateRank' | reverse%}
{% for project in sorted %}
    <li>
    <a href = "{{ project.url}}">{{ project.title }}</a>
    </li>
{% endfor %}
</ul>