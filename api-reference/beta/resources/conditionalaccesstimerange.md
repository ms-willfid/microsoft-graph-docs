---
title: "conditionalAccessTimeRange resource type"
description: "Represents A time range to include in scope of policy."
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

# conditionalAccessTimeRange resource type

Represents A time range to include in scope of policy.

## Properties

| Property | Type | Description |
|:-------- |:---- |:----------- |
| `timeZone` | String | Time zone in +HH:MM or -HH:MM format (ISO 8601). |
| `startDateTime` | String | Start time each day in YYYY-MM-DDTHH:MM:SS format (ISO 8601). |
| `endDateTime` | String | End time each day in YYYY-MM-DDTHH:MM:SS format (ISO 8601). |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "timeZone",
    "startDateTime",
    "endDateTime"
  ],
  "@odata.type": "microsoft.graph.conditionalaccesstimerange"
}-->

```JSON
{
  "timeZone": "String",
  "startDateTime": "String",
  "endDateTime": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditionalaccesstimerange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->