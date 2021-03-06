---
Description: The LINE\_AGENTSTATUSEX message is sent when the status of an ACD agent changes on an agent handler for which the application currently has an open line. This message is generated using lineProxyMessage function.
ms.assetid: a0709367-9105-43af-9772-0161d94c098a
title: LINE_AGENTSTATUSEX message
ms.topic: article
ms.date: 05/31/2018
---

# LINE\_AGENTSTATUSEX message

The **LINE\_AGENTSTATUSEX** message is sent when the status of an ACD agent changes on an agent handler for which the application currently has an open line. This message is generated using [**lineProxyMessage**](/windows/desktop/api/Tapi/nf-tapi-lineproxymessage) function.


```C++
        
```



## Parameters

<dl> <dt>

*dwDevice* 
</dt> <dd>

The application's handle to the line device. This relates to the agent handler.

</dd> <dt>

*dwCallbackInstance* 
</dt> <dd>

The callback instance supplied when opening the line.

</dd> <dt>

*dwParam1* 
</dt> <dd>

The handle of the agent whose status has changed.

</dd> <dt>

*dwParam2* 
</dt> <dd>

Specifies the queue status that has changed. Can be one or more of the [**LINEQUEUESTATUS\_ constants**](linequeuestatus--constants.md).

</dd> <dt>

*dwParam3* 
</dt> <dd>

If *dwParam2* includes the LINEAGENTSTATUSEX \_STATE bit, *dwParam3* indicates the new value of the agent state, which is one of the [**LINEAGENTSTATEEX\_ constants**](lineagentstateex--constants.md).

Otherwise, *dwParam3* is set to zero.

</dd> </dl>

## Requirements



|                         |                                                                                   |
|-------------------------|-----------------------------------------------------------------------------------|
| TAPI version<br/> | Requires TAPI 2.2<br/>                                                      |
| Header<br/>       | <dl> <dt>Tapi.h</dt> </dl> |



## See also

<dl> <dt>

[**lineGetAgentInfo**](/windows/desktop/api/Tapi/nf-tapi-linegetagentinfo)
</dt> <dt>

[**lineProxyMessage**](/windows/desktop/api/Tapi/nf-tapi-lineproxymessage)
</dt> </dl>

 

 




