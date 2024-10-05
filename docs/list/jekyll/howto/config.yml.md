---
layout: default
mx:
  ref:
    - dsl/var/content
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll }}` > _config.yml

# define a layout for content type
```yaml
# Applies to all content types (ie. page, post, collection) 
defaults:
  -
    scope:
      path: "" # Applies to all files
    values:
      layout: "project"
```

```yaml
# apply only to content type "page"
  -
    scope:
      path: "" # Applies to all files
      type: "pages"
    values:
      layout: "project"
```

