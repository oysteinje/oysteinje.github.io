---
layout: default
title:  Index
---

# INDEX

<ul>
  {%- for post in site.posts -%}
  <li>
    {%- assign date_format = "%Y-%m-%d" -%}
    [ {{ post.date | date: date_format }} ] <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
  </li>
	{%- endfor -%}
</ul>
