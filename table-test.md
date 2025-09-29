---
title: Table test
---

The following (test) page is heavily inspired by [this tutorial](https://jekyllrb.com/tutorials/csv-to-table/).

<table>
  {% for row in site.data.authors %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
