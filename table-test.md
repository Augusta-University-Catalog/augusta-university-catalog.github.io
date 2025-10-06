---
title: Table test
---

<!--
_includes/head-custom.html
was edited to load some datatables.net scripts.
-->

The following (test) page is heavily inspired by [this tutorial](https://jekyllrb.com/tutorials/csv-to-table/).

<table id="myTable" class="display">
  {% for row in site.data.augusta_university_courses_2025_10_03_19_51_45
 %}
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

<script> 
$(document).ready( function () {
    $('#myTable').DataTable();
} );
</script>
