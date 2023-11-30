---
layout: home
---

* [ETFs](etfs.md).

{% for file in site.stocks %}
{% assign len = file.path | size %}
* [{{file.path | slice: 15, len | replace: '_', ' ' | remove: '.md'}}]({{file.path | remove: '.md'}}.html)
{% endfor %}
