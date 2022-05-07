---
title: "Create zebraFotaArtifact"
description: "Create a new zebraFotaArtifact object."
author: "dougeby"
localization_priority: Normal
ms.prod: "intune"
doc_type: apiPageType
---

# Create zebraFotaArtifact

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Create a new [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) object.

## Prerequisites
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementConfiguration.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/zebraFotaArtifacts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
In the request body, supply a JSON representation for the zebraFotaArtifact object.

The following table shows the properties that are required when you create the zebraFotaArtifact.

|Property|Type|Description|
|:---|:---|:---|
|id|String|Id of ZebraFotaArtifact.|
|deviceModel|String|Artifact device model.|
|osVersion|String|Artifact OS version.|
|patchVersion|String|Artifact patch version.|
|boardSupportPackageVersion|String|The version of the Board Support Package.|
|releaseNotesUrl|String|Artifact release notes URL.|



## Response
If successful, this method returns a `201 Created` response code and a [zebraFotaArtifact](../resources/intune-androidfotaservice-zebrafotaartifact.md) object in the response body.

## Example

### Request
Here is an example of the request.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/zebraFotaArtifacts
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "deviceModel": "Device Model value",
  "osVersion": "Os Version value",
  "patchVersion": "Patch Version value",
  "boardSupportPackageVersion": "Board Support Package Version value",
  "releaseNotesUrl": "https://example.com/releaseNotesUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 360

{
  "@odata.type": "#microsoft.graph.zebraFotaArtifact",
  "id": "37305f61-5f61-3730-615f-3037615f3037",
  "deviceModel": "Device Model value",
  "osVersion": "Os Version value",
  "patchVersion": "Patch Version value",
  "boardSupportPackageVersion": "Board Support Package Version value",
  "releaseNotesUrl": "https://example.com/releaseNotesUrl/"
}
```



