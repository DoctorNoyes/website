---
class:
  - Literature
area:
  - research
project: 
reading-status: unread
tags: {% if allTags %}{{allTags}}{% endif %}
citekey: {{citekey}}
aliases:
Authors: {{authors}}{{directors}}
---

> **Title**:: {{title}}  
> **Year**:: {{date | format("YYYY")}}  
> **Authors**: {{authors}}{{directors}}  
> **Citekey**:: {{citekey}} {%- if itemType %}  
> **itemType**:: {{itemType}}{%- endif %}{%- if itemType == "journalArticle" %}  
> **Journal**:: *{{publicationTitle}}* {%- endif %}{%- if volume %}  
> **Volume**:: {{volume}} {%- endif %}{%- if issue %}  
> **Issue**:: {{issue}} {%- endif %}{%- if itemType == "bookSection" %}  
> **Book**:: {{publicationTitle}} {%- endif %}{%- if publisher %}  
> **Publisher**:: {{publisher}} {%- endif %}{%- if place %}  
> **Location**:: {{place}} {%- endif %}{%- if pages %}  
> **Pages**:: {{pages}} {%- endif %}{%- if DOI %}  
> **DOI**:: {{DOI}} {%- endif %}{%- if ISBN %}  
> **ISBN**:: {{ISBN}} {%- endif %}    

{%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}  
[Link](file://{{attachment.path | replace(" ", "%20")}}) {%- endfor -%}.
## Abstract

{%- if abstractNote %}  
{{abstractNote}}  
{%- endif -%}.

---
Contribution::

Related: 

---
