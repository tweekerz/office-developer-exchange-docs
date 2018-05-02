---
title: "StartTime"
 
 
manager: sethgros
ms.date: 9/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: "The StartTime element represents the start of a time span."
---

# StartTime

The **StartTime** element represents the start of a time span. 
  
```
<StartTime/
```

 **dateTime**
## Attributes and elements

The following sections describe attributes, child elements, and parent elements.
  
#### Attributes

None.
  
#### Child elements

None.
  
#### Parent elements

|**Element**|**Description**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |Identifies the time span queried for the user availability information.  <br/> The following is the XPath expression to this element:  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifies the time span that is queried for detailed information about suggested meeting times.  <br/> The following is the XPath expression to this element:  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> | Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.  <br/>  The following are the possible XPath expressions to this element:  <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |Represents a unique calendar item occurrence. This is used for Availability inquiries. The **StartTime** element is required in the **CalendarEvent** element. The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.  <br/> The following is the XPath expression to this element:  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## Text value

A text value is required.
  
## Remarks

The [EndTime](endtime.md) element represents the end of the time span. 
  
The schema includes many [StartTime](starttime.md) elements. 
  
> [!NOTE]
> The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed. 
  
## Element information

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Schema Name  <br/> |Types schema  <br/> |
|Validation File  <br/> |Types.xsd  <br/> |
|Can be Empty  <br/> |False  <br/> |
   
## See also

#### Reference

[GetUserAvailability operation](getuseravailability-operation.md)
#### Other resources

[Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
