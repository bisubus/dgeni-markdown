{%- if doc.params %}

### Arguments

| Param | Type | Details |
| :--: | :--: | :--: |
{%- for param in doc.params %}
| {$ param.name | esc $} {%- if param.type.optional %}<br>*(optional)*{% endif %} | {$ param.type.name $} | {$ param.description | esc | marked | nobr $} |{% endfor -%}

{%- endif -%}
