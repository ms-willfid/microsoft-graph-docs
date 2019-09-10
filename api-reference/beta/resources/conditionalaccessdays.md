---
title: "conditionalAccessDays resource type"
description: "Represents the days of the week and times to include in the scope of policy."
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

# conditionalAccessDays resource type

Represents the days of the week and times to include in the scope of policy.

## Properties

| Property | Type | Description |
|:-------- |:---- |:----------- |
| `daysOfWeek` | dayOfWeek collection | The days of the week that are included. Possible values: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday`, `Saturday`. |
| `timeZone` | String | Time zone in +HH or -HH format (ISO 8601). |
| `startTime` | String | Start time each day in HH:MM:SS format (ISO 8601). |
| `endTime` | String | End time each day in HH:MM:SS format (ISO 8601). |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "daysOfWeek",
    "timeZone",
    "startTime",
    "endTime"
  ],
  "@odata.type": "microsoft.graph.conditionalaccessdays"
}-->

```JSON
{
  "daysOfWeek": [ "String" ],
  "timeZone": "String",
  "startTime": "String",
  "endTime": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditionalaccessdays resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->