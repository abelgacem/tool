---
layout: default
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}`

# definition
- set of a kvpair.
- Used at Build time by jekyll itself.
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
  title:  'about'
  categorizations: 'cat01 cat02'
  permalink: '/:category'
```

# list
|name|type|description|
|-|-|-|
|layout||a page's CSS.|
|title||a browser's tab name.|
|permalink|parameterized|a page's URL.|
|catagories|seq. of string|
