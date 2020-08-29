---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

WHAT IS THIS ???

    <footer>
        <a class="active" href="#">{{ site.languageNames[site.lang] }}</a>
        {% for lang in site.languageNames %}
        {% if lang[0] == site.lang %} {% continue %} {% endif %}
        {% if page.namespace %}
        <a href="{% tl {{ page.namespace }} {{ lang[0] }} %}">{{ lang[1] }}</a>
        {% else %}
        <a href="{{ site.baseurl_root }}/{{ lang[0] }}/">{{ lang[1] }}</a>
        {% endif %}
        {% endfor %}
    </footer>