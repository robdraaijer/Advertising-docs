---
title: NegativeSite Data Object - Campaign Management
ms.service: bing-ads-campaign-management-service
ms.topic: article
author: eric-urban
ms.author: eur
description: Reserved.
---
# NegativeSite Data Object - Campaign Management
Reserved.

## Syntax
```xml
<xs:complexType name="NegativeSite" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:complexContent mixed="false">
    <xs:extension base="tns:SharedListItem">
      <xs:sequence>
        <xs:element minOccurs="0" name="Id" nillable="true" type="xs:long" />
        <xs:element minOccurs="0" name="Url" nillable="true" type="xs:string" />
      </xs:sequence>
    </xs:extension>
  </xs:complexContent>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="id"></a>Id|Reserved.|**long**|
|<a name="url"></a>Url|Reserved.|**string**|

The [NegativeSite](negativesite.md) object has [Inherited Elements](#inheritedelements).

## <a name="inheritedelements"></a>Inherited Elements

### <a name="inheritedelementssharedlistitem"></a>Inherited Elements from SharedListItem
The [NegativeSite](negativesite.md) object derives from the [SharedListItem](sharedlistitem.md) object, and inherits the following elements. The descriptions below are specific to [NegativeSite](negativesite.md), and might not apply to other objects that inherit the same elements from the [SharedListItem](sharedlistitem.md) object.  

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="forwardcompatibilitymap"></a>ForwardCompatibilityMap|Reserved.|[KeyValuePairOfstringstring](keyvaluepairofstringstring.md) array|
|<a name="type"></a>Type|Reserved.|**string**|

## Requirements
Service: [CampaignManagementService.svc v13](https://campaign.api.bingads.microsoft.com/Api/Advertiser/CampaignManagement/v13/CampaignManagementService.svc)  
Namespace: https\://bingads.microsoft.com/CampaignManagement/v13  

