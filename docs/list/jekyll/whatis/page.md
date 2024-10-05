---
layout: default
mx:
  ref:
    - dsl/var/content
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll }}` > `page`

# definition
- Text file written in `markdown`.
- Content contribute to output 1 `html` page when building the artifact (aka. the site)

# Type
- [Not]Draft

# Toknow
- a page can simply be added to the root folder
  - it will output by default an `html` file with 
    - path`${siteUrl}/${PageName}`
  - if the frontmater:key:permalink exists the url will be **`${permalink}`**
- a page can also be organized into folders

# Rules
