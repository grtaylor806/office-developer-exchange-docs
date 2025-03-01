---
title: "GetStreamingEventsResponseMessage"
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: "The GetStreamingEventsResponseMessage element contains the status and result of a single GetStreamingEvents operation request."
---

# GetStreamingEventsResponseMessage

The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request. 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 **GetStreamingEventsResponseMessageType**
## Attributes and elements

The following sections describe attributes, child elements, and parent elements.
  
### Attributes

|**Attribute**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response. <br/><br/>The following values are valid for this attribute:  <br/><br/>-  Success  <br/>-  Warning  <br/>-  Error  <br/> |
   
#### ResponseClass Attribute

|**Value**|**Description**|
|:-----|:-----|
|Success  <br/> |Describes a request that is fulfilled.  <br/> |
|Warning  <br/> | Describes a request that was not processed. A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed. <br/><br/>The following are examples of sources of warnings:  <br/><br/>-  The Exchange store is offline during the batch.  <br/>-  Active Directory Domain Services (AD DS) is offline.  <br/>-  Mailboxes were moved.  <br/>-  The mailbox database (MDB) is offline.  <br/>-  A password has expired.  <br/>-  A quota was exceeded.  <br/> |
|Error  <br/> | Describes a request that cannot be fulfilled. <br/><br/>The following are examples of sources of errors:  <br/><br/>-  Invalid attributes or elements  <br/>-  Attributes or elements that are out of range  <br/>-  An unknown tag  <br/>-  An attribute or element that is not valid in the context  <br/>-  An unauthorized access attempt by any client  <br/>-  A server-side failure in response to a valid client-side call  <br/><br/>  Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.  <br/> |
   
### Child elements

|**Element**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Provides a text description of the status of the response.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Provides an error code that identifies the specific error that the request encountered.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Currently unused and is reserved for future use. It contains a value of 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Provides additional error response information.  <br/> |
|[Notifications](notifications.md) <br/> |Contains a list of information about the subscription and the events that have occurred since the last notification.  <br/> |
|[ErrorSubscriptionIds](errorsubscriptionids.md) <br/> |Contains a list of subscription IDs that are invalid.  <br/> |
|[ConnectionStatus](connectionstatus.md) <br/> |Provides a text description of the status of a streaming subscription.  <br/> |
   
### Parent elements

|**Element**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contains the response messages for an Exchange Web Services request.  <br/> |
   
## Text value

None.
  
## Remarks

The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).
  
## Element information

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Schema Name  <br/> |Messages schema  <br/> |
|Validation File  <br/> |Messages.xsd  <br/> |
|Can be Empty  <br/> |False  <br/> |
   
## See also

- [GetStreamingEvents](getstreamingevents.md) 
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
- [GetStreamingEvents operation](getstreamingevents-operation.md)

