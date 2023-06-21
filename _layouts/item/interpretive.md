---
# generic fallback item page layout 
# displays image or icon depending on "image_thumb"
layout: about
---
{% assign essay = page.objectid %}
{% capture interpretive-content%}{% include interpretive/{{essay}}.md %}{% endcapture %}

<h2>{{page.title}}</h2>

{{interpretive-content | markdownify }}
