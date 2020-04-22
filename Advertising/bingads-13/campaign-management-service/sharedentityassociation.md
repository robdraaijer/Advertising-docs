---
title: SharedEntityAssociation Data Object - Campaign Management
ms.service: bing-ads-campaign-management-service
ms.topic: article
author: eric-urban
ms.author: eur
description: Defines an object that associates a campaign to negative keyword list, or an ad account to a website exclusion list.
---
# SharedEntityAssociation Data Object - Campaign Management
Defines an object that associates a campaign to negative keyword list, or an ad account to a website exclusion list.

## Syntax
```xml
<xs:complexType name="SharedEntityAssociation" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:sequence>
    <xs:element name="EntityId" type="xs:long" />
    <xs:element minOccurs="0" name="EntityType" nillable="true" type="xs:string" />
    <xs:element minOccurs="0" name="SharedEntityCustomerId" nillable="true" type="xs:long">
      <xs:annotation>
        <xs:appinfo>
          <DefaultValue EmitDefaultValue="false" xmlns="http://schemas.microsoft.com/2003/10/Serialization/" />
        </xs:appinfo>
      </xs:annotation>
    </xs:element>
    <xs:element name="SharedEntityId" type="xs:long" />
    <xs:element minOccurs="0" name="SharedEntityType" nillable="true" type="xs:string" />
  </xs:sequence>
</xs:complexType>
```

## <a name="elements"></a>Elements

|Element|Description|Data Type|
|-----------|---------------|-------------|
|<a name="entityid"></a>EntityId|The identifier of the campaign or ad account (according to [EntityType](#entitytype)) that is associated with the shared entity.|**long**|
|<a name="entitytype"></a>EntityType|The type of entity.<br/><br/>This element must be set to "Campaign" for negative keyword list to campaign associations in your ad account shared library.<br/><br/>This element must be set to "Account" for website exclusion list to ad account associations in your manager account (customer) shared library.|**string**|
|<a name="sharedentitycustomerid"></a>SharedEntityCustomerId|Determines the owner of a website exclusion list.<br/><br/>This read-only element is only available for [PlacementExclusionList](placementexclusionlist.md) associations. You can view all list associations for accounts that you can access. However, only the owner of the list can associate and disassociate it with ad accounts.|**long**|
|<a name="sharedentityid"></a>SharedEntityId|The identifier of the shared entity.|**long**|
|<a name="sharedentitytype"></a>SharedEntityType|The type of shared entity.<br/><br/>This element must be set to "NegativeKeywordList" for negative keyword list to campaign associations in your ad account shared library.<br/><br/>This element must be set to "PlacementExclusionList" for website exclusion list to ad account associations in your manager account (customer) shared library.|**string**|

## Requirements
Service: [CampaignManagementService.svc v13](https://campaign.api.bingads.microsoft.com/Api/Advertiser/CampaignManagement/v13/CampaignManagementService.svc)  
Namespace: https\://bingads.microsoft.com/CampaignManagement/v13  

## Used By
[DeleteSharedEntityAssociations](deletesharedentityassociations.md)  
[GetSharedEntityAssociationsByEntityIds](getsharedentityassociationsbyentityids.md)  
[GetSharedEntityAssociationsBySharedEntityIds](getsharedentityassociationsbysharedentityids.md)  
[SetSharedEntityAssociations](setsharedentityassociations.md)  
