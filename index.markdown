---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page 
---
<ul class="post-list">
 {% for post in site.posts %}
  <li>
   <span class="post-meta">{{ post.date | date_to_string: "ordinal", "US" }}</span>
   <h3>
   <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
   </h3>
   {{ post.excerpt }}
  </li>
 {% endfor %}
</ul>
