---
title: "skypeForBusinessActivityUserCounts resource type"
description: "The following is a JSON representation of the resource."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ""
author: "kszb"
---

# skypeForBusinessActivityUserCounts resource type

Namespace: microsoft.graph

## Properties

| Property          | Type   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| organized         | Int64  |
| participated      | Int64  |
| reportRefreshDate | Date   |
| reportDate        | Date   |
| reportPeriod      | String |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024,
  "organized": 1024,
  "participated": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


