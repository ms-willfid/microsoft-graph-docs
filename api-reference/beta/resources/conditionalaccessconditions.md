---
title: "conditionalAccessConditions resource type"
description: "Represents the type of conditions that govern when the policy applies."
localization_priority: Normal
author: "davidmu1"
ms.prod: "microsoft-identity-platform"
doc_type: resourcePageType
---

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

# conditionalAccessConditions resource type

Represents the type of conditions that govern when the policy applies.

## Properties

| Property | Type | Description |
|:-------- |:---- |:----------- |
| `signInRiskLevels` | riskLevel collection | Risk levels included in the policy scope. Possible values: `High`, `Medium`, `Low`, `None`. |
| `clientAppTypes` | conditionalAccessClientApps collection | Client application types included in the policy scope. Possible values: `Browser`, `Modern`, `EasSupported`, `EasUnsupported`, `Other`. |
| `applications` | [conditionalAccessApplications](conditionalaccessapplications.md) | Applications and ACRS tags included in and excluded from the policy scope. Required. |
| `users` | [conditionalAccessUsers](conditionalaccessusers.md) | Users, groups, and roles included in and excluded from the policy scope. Required. |
| `platforms` | conditionalAccessPlatforms | Platforms included in and excluded from the policy scope. Possible values: `All`, `Android`, `Ios`, `Windows`, `WindowsPhone`, `MacOs`. |
| `locations` | [conditionalAccessLocations](conditionalaccesslocations.md) | Locations included in and excluded from the policy scope. |
| `times` | [conditionalAccessTimes](conditionalaccesstimes.md) | Times in scope of the policy. |
| `deviceStates` | [conditionalAccessDeviceStates](conditionalaccessdevicestates.md) | Device states in the policy scope. |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "signInRiskLevels",
    "clientAppTypes",
    "applications",
    "users",
    "platforms",
    "locations",
    "times",
    "deviceStates"
  ],
  "@odata.type": "microsoft.graph.conditionalaccessconditions"
}-->

```json
{
  "signInRiskLevels": [ "String" ],
  "clientAppTypes": [ "String" ],
  "applications": { "@odata.type": "microsoft.graph.conditionalaccessapplications" },
  "users": { "@odata.type": "microsoft.graph.conditionalaccessusers" },
  "platforms": "String",
  "locations": { "@odata.type": "microsoft.graph.conditionalaccesslocations" },
  "times": { "@odata.type": "microsoft.graph.conditionalaccesstimes" },
  "deviceStates": { "@odata.type": "microsoft.graph.conditionalaccessdevicestates" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditionalaccessconditions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->