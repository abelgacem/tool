---
layout: default
mx:
  lp:
  ref:
    - whatis/tag
---



# Create 
- This create a folder that is a 
  - `Git` project (ie. repo) 
  - `Ruby gems`
  - Jekyll theme
```shell
# var
lTHEME_NAME="mxtheme01"
jekyll new-theme ${mxtheme01}
```
- update the file `xxx.gempspec`
- install the dependencies neeeded by this gems
```shell
# install the gems defined in the Gemfile of the project
bundle install
```

Create the gem
```shell
# create the file ${lTHEME_NAME}-${version}.gem is created
gem build ${lTHEME_NAME}.gemspec  
```

# install locally
```shell ${lTHEME_NAME}-${version}.gem
gem install 
```
meaning:
  - install this gem in the local ruby gem repository.
  - this repository is `$(gem env | grep -i install | grep -iv user)`

# Declare
```shell
# add dependency in Gemfile
gem "mythme", "~> 2.2"

# declare it in _config.yml
theme: minima
```

# update dependencies
```shell
# in Gemfile
bundle install
```