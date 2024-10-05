---
layout: default
mx:
  ref:
    - dsl/var/content
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll }}` > post

# define
```yaml
# in _config.yml
collections:
  my_collection:
    output: true
    permalink: /:collection/:name
```
