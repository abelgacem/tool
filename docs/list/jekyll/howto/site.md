---
layout: default
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}` > Howto

# Create a site
```shell
lJEKYLL_SITE="${HOME}/wkspc/jekyll/site00"
lJEKYLL_SITE="/tmp/site00"
mkdir -p $(dirname ${lJEKYLL_SITE})
jekyll new ${lJEKYLL_SITE} 
``` 

# Build a site
```shell
cd ${lJEKYLL_SITE}
bundle exec jekyll build
``` 

# Build (if needed) and publish a site
```shell
cd ${lJEKYLL_SITE}
bundle exec jekyll serve --livereload --incremental
``` 
meaning:
- `--livereload`:  a changes trigger a build and a publish
- `--incremental`: build is incremental


# Browse a site
```shell
localhost:4000
``` 
