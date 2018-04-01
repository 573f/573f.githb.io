---
layout: default
title: "Blog"
permalink: "/blog/"
---
{% for post in site.posts %}
## {{ post.title }}
#### {{ post.subtitle }}
_{{ post.date | date: '%B %d, %Y' }}_
 
{{ post.excerpt | remove: '<p>' | remove: '</p>' }}
[-- more --]({{ post.url }})
{% endfor %}
