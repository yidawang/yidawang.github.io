---
layout: default
---

<section id="about">
{% capture about_content %}{% include_relative about.md %}{% endcapture %}
{{ about_content | markdownify }}
</section>