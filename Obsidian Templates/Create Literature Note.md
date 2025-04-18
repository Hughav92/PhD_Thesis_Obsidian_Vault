#literature-note 

---
category:: literaturenote
tags:: {% set tags = allTags.split(',') %}{% for tag in tags %}#{{tag|trim|replace(" ", "-")|replace(".","")|replace("&", "and")}} {% endfor %}
status:: {% if allTags %}{% if "read" in allTags and "unread" not in allTags %}{{"read"}}{% else %}{{"unread"}}{% endif %} {% else %}{{"unread"}}{% endif %}
dateread::
reference:: {{bibliography}}

---

> [!Cite]
> {{bibliography}}
^cite

>[!Synth]
>{% persist "synth" %}{% if isFirstImport %}
>
>**Contribution**:: 
>
>**Related**::  {% for relation in relations | selectattr("citekey") %} [[@{{relation.citekey}}]]{% if not loop.last %}, {% endif%} {% endfor %}
>{% endif %}{% endpersist %}

>[!md]
{% for type, creators in creators | groupby("creatorType") -%}
{%- for creator in creators -%}
> **{{"First" if loop.first}}{{type | capitalize}}**::
{%- if creator.name %} {{creator.name}}  
{%- else %} {{creator.lastName}}, {{creator.firstName}}  
{%- endif %}  
{% endfor %}~ 
{%- endfor %}    
> **Title**:: {{title}}  
> **Year**:: {{date | format("YYYY")}}   
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

> [!LINK] 
> {%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}
> [[{{attachment.title}}]]  {%- endfor -%}.

> [!Abstract]
> {%- if abstractNote %}
> {{abstractNote}}
> {%- endif -%}.
> 
# Notes

{% persist "notes" %}{% if isFirstImport %}
{% endif %}
{%- if markdownNotes %}
{{markdownNotes}}
{%- endif %}
{% endpersist %}


# Annotations
{%- macro calloutHeader(type, color) -%}  
{%- if type == "highlight" -%}  
<mark style="background-color: {{color}}">Quote</mark>  
{%- endif -%}

{%- if type == "text" -%}  
Note  
{%- endif -%}  
{%- endmacro -%}

{% persist "annotations" %}
{% set newAnnotations = annotations | filterby("date", "dateafter", lastImportDate) %}
{% if newAnnotations.length > 0 %}

### Imported: {{importDate | format("YYYY-MM-DD h:mm a")}}

{% for a in newAnnotations %}
{{calloutHeader(a.type, a.color)}}
> {{a.annotatedText}}
{% endfor %}
{% endif %}
{% endpersist %}

{% if attachments %}
{% set images_displayed = false %}
{% for attachment in attachments %}
{% set ext = attachment.path.split('.')|last %}
{% if ext in ['png', 'jpg', 'jpeg', 'svg', 'gif', 'tiff', 'bmp'] %}
{% if not images_displayed %}
# Images
{% set images_displayed = true %}
{% endif %} 
![[{{attachment.title}}.{{ext}}]]
From [[@{{citekey}}]]

{% endif %}
{% endfor %}
{% endif %}