---
layout: index
title:  myIndex
---
[link]:        #
[repo_source]: #


<!-- define var -->
{% assign lLIST_PAGE         = site.pages %}

# {{ site.data.name.introduction }}
- This documentation is built and deployed from a [GitHub repository][repo_source].

# {{ site.data.name.purpose }}
- Document IT {{ site.mx.domain | append: "s"}}.


# List


<!-- <table id="myTable"> -->
<table class="sortable">
  <thead>
    <tr>
      <th>project name</th>
      <th translate='no'>tag</th>
      <th>description</th>
      <th>path</th>
    </tr>
  </thead>
  <tbody>
    {% for lPAGE in lLIST_PAGE %}
      {% assign lITEM_NAME = lPAGE.path | split: "/" | slice: 1, 1 | first | downcase | strip %}
      {% if lITEM_NAME != "" %}
      <tr>
        <td translate='no'><a href="{{ lPAGE.path | remove: '.md' }}">{{ lITEM_NAME }}</a></td>
        <td translate='no'>{{ lPAGE.mx.domain }}</td>
        <td>{{ lPAGE.mx.description }}</td>
        <td>{{ lPAGE.path }}</td>
      </tr>
      {% endif %}
    {% endfor %}
  </tbody>
</table>


