---
title: "Get accessPackageCatalog"
description: "Retrieve the properties and relationships of accesspackagecatalog object."
author: "markwahl-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---
# Get accessPackageCatalog

Namespace: microsoft.graph


Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}
```

## Optional query parameters

This method supports the `$select` and `$expand` OData query parameters to help customize the response. To retrieve the access packages in a catalog, include `$expand=accessPackages` in the query. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name      |Description|
|:----------|:----------|
| Authorization | Bearer \{token\}. Required. |

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs/b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1",
  "displayName": "Access package catalog for testing",
  "description": "Sample access package catalog",
  "catalogType": "userManaged",
  "state": "published",
  "isExternallyVisible": false,
  "createdDateTime": "2019-01-27T18:19:50.74Z",
  "modifiedDateTime": "2019-01-27T18:19:50.74Z"
}
```


