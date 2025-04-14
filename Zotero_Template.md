---
tags: {% if allTags %}{{allTags}}{% endif %}
created: {{importDate|format("YYYY-MM-DD")}}
---


### Titel: {{title}}

**Authors:** {{authors}}

**Reference:** {{bibliography}}
**Zotero Link:** {{pdfZoteroLink}}

> [!NOTE]- Abstract
> {{abstractNote}}


{% for annotation in annotations -%} 
{%- if annotation.annotatedText -%}*{{annotation.annotatedText}}*([p.{{annotation.pageLabel}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.pageLabel}}&annotation={{annotation.id}}))
{% endif %}{% if annotation.imageRelativePath %}![[{{annotation.imageRelativePath}}]]{% endif %}
{% if annotation.comment %}{{annotation.comment}}{%- endif %} 
{% if annotation.hashTags %}{{annotation.hashTags}}{%- endif %} 

{% endfor %}