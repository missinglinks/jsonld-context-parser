# Json-LD utils

Helpers for JSON-LD processing.

## Json-LD Context Mapper

Maps terms and namespaces/uris in an Json-LD context file.

Use:

```
from json_utils import JsonLDContextMapper 

#context file as url
cm = JsonLDContextMapper("https://linked.art/ns/v1/linked-art.json")

#local context file
cm = JsonLDContextMapper("data/context.json")

#get term URIRef object
uri = cm["shows"]
#OUT: http://www.cidoc-crm.org/cidoc-crm/P65_shows_visual_item

```