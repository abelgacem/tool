---
layout: default
---


[//]: #(Reference)
[homepage]:   {{ "/index" | absolute_url }}

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}` > Howto
# Install on ubuntu
- install os dependency
```shell
sudo apt-get -y install ruby-full build-essential zlib1g-dev
```
- export envvar
```shell
# define var
export GEM_HOME="${HOME}/wkspc/gems"
export PATH="${GEM_HOME}/bin:$PATH"
```

- install tool
```shell
# define var
gem install jekyll bundler
```
# Create a site
```shell
lJEKYLL_SITE="${HOME}/wkspc/jekyll/site00"
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
bundle exec jekyll serve --livereload
``` 

