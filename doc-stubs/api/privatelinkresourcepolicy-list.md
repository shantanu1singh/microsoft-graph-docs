---
title: "List privateLinkResourcePolicies"
description: "Get a list of the privateLinkResourcePolicy objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List privateLinkResourcePolicies
Namespace: microsoft.graph

Get a list of the [privateLinkResourcePolicy](../resources/privatelinkresourcepolicy.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policyRoot/privateLinkResourcePolicies
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [privateLinkResourcePolicy](../resources/privatelinkresourcepolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_privatelinkresourcepolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policyRoot/privateLinkResourcePolicies
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.privateLinkResourcePolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.privateLinkResourcePolicy",
      "id": "6b715b25-5b25-6b71-255b-716b255b716b",
      "externalPrivateLinkId": "String",
      "tenantApprovals": [
        {
          "@odata.type": "microsoft.graph.tenantApprovals"
        }
      ]
    }
  ]
}
```
