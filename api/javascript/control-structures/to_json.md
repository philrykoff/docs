---
layout: api-command
language: JavaScript
permalink: api/javascript/to_json/
command: toJson
io:
    -   - any
        - string
related_commands:
    json: json/
---
# Command syntax #

{% apibody %}
any.toJson(value) &rarr; string
{% endapibody %}

# Description #

Convert a ReQL value or object to a JSON string.

__Example:__ Get a ReQL document as a JSON string.

```js
> r.table('hero').get(1).toJson()
// result returned to callback
'{"id": 1, "name": "Batman", "city": "Gotham", "powers": ["martial arts", "cinematic entrances"]}'
```