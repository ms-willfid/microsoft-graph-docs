---
title: "conditionalAccessLocations resource type"
description: "Represents locations included in and excluded from the policy scope."
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

# conditionalAccessLocations resource type

Represents locations included in and excluded from the policy scope.

## Properties

| Property | Type | Description |
|:-------- |:---- |:----------- |
| `includeLocations` | String collection | Location IDs in scope of policy unless explicitly excluded, `ALL`, or `AllTrusted`. |
| `excludeLocations` | String collection | Location IDs excluded from scope of policy. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalaccesslocations"
}-->

```JSON
{
  "includeLocations": [ "String" ],
  "excludeLocations": [ "String" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditionalaccesslocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->