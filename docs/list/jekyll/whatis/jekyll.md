---
layout: default
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll }}`

# Definition
- {{ site.data.tool_description.jekyll }}
- A framework.
- A static web site generator.
- written in ruby.
- Uses `Liquid` as templating language.

# The Process
- Create an empty `jekyll` project.
  - This generate a basic directory structure.
- Make changes inside this folder by upfating `Jekyll` objects and custom contents like:
  - layout
  - content  
- Build the project. This consist of the following tasks
  - set up plugins
  - read src file.
  - run generators.
  - render template.
  - write file to disk (ie.output the artifact : a folder named `_site`)
- Deploy the artifact and browse the site:
  - In a local environment while coding.
  - In any shared other environment (eg. dev, test, pprod, prod) for testing.

