---
title: "Update unifiedRoleEligibilityRequest"
description: "Update the properties of an unifiedRoleEligibilityRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRoleEligibilityRequest
Namespace: microsoft.graph

Update the properties of an [unifiedRoleEligibilityRequest](../resources/unifiedroleeligibilityrequest.md) object.

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
PATCH /unifiedRoleEligibilityRequests/{unifiedRoleEligibilityRequestsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [unifiedRoleEligibilityRequest](../resources/unifiedroleeligibilityrequest.md) object.

The following table shows the properties that are required when you update the [unifiedRoleEligibilityRequest](../resources/unifiedroleeligibilityrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [request](../resources/request.md)|
|action|String|**TODO: Add Description**|
|principalId|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|
|directoryScopeId|String|**TODO: Add Description**|
|appScopeId|String|**TODO: Add Description**|
|isValidationOnly|Boolean|**TODO: Add Description**|
|targetScheduleId|String|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|**TODO: Add Description**|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [unifiedRoleEligibilityRequest](../resources/unifiedroleeligibilityrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleeligibilityrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/unifiedRoleEligibilityRequests/{unifiedRoleEligibilityRequestsId}
Content-Type: application/json
Content-length: 467

{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityRequest",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityRequest",
  "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```
