---
layout: default
title: Home
---

# Welcome to My Jekyll Site  

Bu, Jekyll sitemin ana sayfasıdır. En son blog yazılarımı aşağıda görebilirsiniz:

---

## Blog Yazıları  
{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})**  
  *{{ post.date | date: "%d %B %Y" }}*  
  {{ post.excerpt }}
{% endfor %}
