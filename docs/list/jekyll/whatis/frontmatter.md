---
layout: default
mx:
  lp:
  ref:
    - def/content
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}`

# definition
- set of a kvpair or variable.
- define in the begining of a content.
- Used at build time by jekyll.
- Can be used by a markdown's code to control the final output.

# type
- Sdef, Udef

# Example of frontmatter@sdef
```shell
layout: 'page'
title:  'about'
categorizations: 'cat01 cat02'
permalink: '/:category'
```

# Example of frontmatter@udef
```shell
mx: 
  lp:
  ref:
  var:
    title:  'about'
    tag: 'cat01 cat02'
```

# list
|name|type|description|
|-|-|-|
|layout||a page's CSS.|
|title||a browser's tab name.|
|permalink|parameterized|a page's URL.|
|catagories|seq. of string|
