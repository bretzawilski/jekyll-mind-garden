---
layout: note
title: Evergreen Notes
tags: evergreen
type: note
fileName: evergreen-notes
id: evergreen notes
---

<ul>
    {% for note in site.notes %}
    {% if note.tags[0] == "evergreen" %}
    <li>
	    {% assign title = note.title %}
        [[{{ title | inspect }}]]
    </li>
   {% endif %}
   {% if note.tags[1] == "evergreen" %}
    <li>
        <a href="{{ note.url }}">{{ note.title }}</a>
    </li>
   {% endif %}
   {% if note.tags[2] == "evergreen" %}
    <li>
        <a href="{{ note.url }}">{{ note.title }}</a>
    </li>
    {% endif %}
    {% if note.tags[3] == "evergreen" %}
    <li>
        <a href="{{ note.url }}">{{ note.title }}</a>
    </li>
   {% endif %}
    {% endfor %}
</ul>


