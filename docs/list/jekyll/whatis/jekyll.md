---
layout: default
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}`

# Definition
- A framework.
- A static web site generator.
- written in ruby.
- A DSL.

# The Process
- Create an empty `jekyll` project.
  - This generate a basic directory structure.
- Make changes to this basic site by defining `Jekyll` objects and custom contents:
  - layout
  - page  
  - fontmatter
- Build the project.
  - This will output an artifact : a folder named `_site`
- Deploy the artifact and browse the site:
  - Locally while developing.
  - In test or any other envs (aka. production).