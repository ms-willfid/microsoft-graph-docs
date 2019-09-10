---
title: "conditionalAccessDeviceStates resource type"
description: "Represents device states in the policy scope."
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

# conditionalAccessDeviceStates resource type

Represents device states in the policy scope.

## Properties

| Property | Type | Description |
|:-------- |:---- |:----------- |
| `includeStates` | String collection | States in the scope of the policy. `ALL` is the only allowed value. |
| `excludeStates` | String collection | States excluded from the scope of the policy. Possible values: `Compliant`, `DomainJoined`. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeStates",
    "excludeStates"
  ],
  "@odata.type": "microsoft.graph.conditionalaccessdevicestates"
}-->

```JSON
{
  "includeStates": [ "String" ],
  "excludeStates": [ "String" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditionalaccessdevicestates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->