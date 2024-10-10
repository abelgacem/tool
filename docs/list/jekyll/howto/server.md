---
---


[//]: #(Reference)
[homepage]:   {{ site.baseurl }}/

# [&larr;][homepage] Tool > `{{ site.data.tool_name.jekyll_name }}` > Howto



# Get server status
```shell
[ -n "$(ps -ef | grep jekyll | grep serve | awk '{print $2}')" ] && echo "Server running" || echo "No server running"
``` 
