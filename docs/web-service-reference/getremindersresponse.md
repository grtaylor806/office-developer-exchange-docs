---
title: "GetRemindersResponse"
 
 
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1b1c7288-2a98-4142-8961-4d2ebca5c37c
description: "The GetRemindersResponse element specifies the response to a GetReminders request."
---

# GetRemindersResponse

The **GetRemindersResponse** element specifies the response to a **GetReminders** request. 
  
```XML
<GetRemindersResponse>
   <Reminders></Reminders>
</GetRemindersResponse>

```

 **GetRemindersResponseMessageType**
## Attributes and elements

The following sections describe attributes, child elements, and parent elements.
  
### Attributes

None.
  
### Child elements

[Reminders](reminders.md)
  
### Parent elements

[ResponseMessages](responsemessages.md)
  
## Remarks

This element was introduced in Exchange Server 2013.
  
The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.
  
## Element information

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Schema Name  <br/> |Messages schema  <br/> |
|Validation File  <br/> |Messages.xsd  <br/> |
|Can be Empty  <br/> |False  <br/> |
   
## See also



[ResponseMessages](responsemessages.md)


- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)

