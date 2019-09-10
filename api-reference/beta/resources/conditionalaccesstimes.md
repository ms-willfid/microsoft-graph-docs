---
title: "conditionalAccessTimes resource type"
description: "Represents times in the scope of the policy."
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

# conditionalAccessTimes resource type

Represents times in the scope of the policy.

## Properties

| Property | Type | Description |
|:-------- |:---- |:----------- |
| `allTimes` | Boolean | Apply to all times. If true, overrides all other time and day settings. |
| `includeDays` | [conditionalAccessDays](conditionalaccessdays.md) | Set of days of the week and times to include in scope of policy. |
| `excludeDays` | [conditionalAccessDays](conditionalaccessdays.md) | Set of days of the week and times to exclude from scope of policy. |
| `includeRange` | [conditionalAccessTimeRange](conditionalaccesstimerange.md) | A time range to include in scope of policy. |
| `excludeRange` | [conditionalAccessTimeRange](conditionalaccesstimerange.md) | A time range to exclude from scope of policy. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "excludeDays",
    "includeRange",
    "allTimes",
    "includeDays",
    "excludeRange"
  ],
  "@odata.type": "microsoft.graph.conditionalaccesstimes"
}-->

```JSON
{
  "excludeDays": { "@odata.type": "microsoft.graph.conditionalaccessdays" },
  "includeRange": { "@odata.type": "microsoft.graph.conditionalaccesstimerange" },
  "allTimes": false,
  "includeDays": { "@odata.type": "microsoft.graph.conditionalaccessdays" },
  "excludeRange": { "@odata.type": "microsoft.graph.conditionalaccesstimerange" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditionalaccesstimes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->