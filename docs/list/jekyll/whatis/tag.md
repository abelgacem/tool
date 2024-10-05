---
layout: default
mx:
  lp:
  ref:
    - howto/tag
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}` > `tag`

# definition
- are defined in the front matter
- exists for any content types: `page`, `post`, `collection`

# To know
```yaml
# will be processed as a string
tag: classic hollywood
# will be processed as an array of 2 strings
tags: classic hollywood
```  

# To know
- All tags registered in the current site are exposed to Liquid templates via `site.tags`.
- Iterating over `{{site.tags}`} on a page will yield another array with two items
  - first item is the name of the tag
  - second item is an array of posts with that tag.