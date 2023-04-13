{% if include.low %}###{% else %}##{% endif%} {{ include.name }}

{% if include.begriffe %}|Kernbegriffe|{{ include.begriffe }}|{% endif %}{% if include.zeit %}
|Zeit|{{ include.zeit }}|{% endif %}{% if include.ereignisse %}
|Wichtige Ereignisse|{{ include.ereignisse }}|{% endif %}{% if include.literatur %}
|Literatur|{{ include.literatur }}{% endif %}{% if include.werke %}
|Werke|{{ include.werke }}|{% endif %}
