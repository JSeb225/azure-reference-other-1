# IoTHubClient_LL_SendReportedState()

This API sneds a report of the device's properties and their current values.

## Syntax

\#include "[azure-iot-sdk-c/iothub_client/inc/iothub_client_ll.h](../iot-c-ref-iothub-client-ll-h.md)"  
```C
IOTHUB_CLIENT_RESULT IoTHubClient_LL_SendReportedState(
  IOTHUB_CLIENT_LL_HANDLE                iotHubClientHandle,
  const unsigned char *                  reportedState,
  size_t                                 size,
  IOTHUB_CLIENT_REPORTED_STATE_CALLBACK  reportedStateCallback,
  void *                                 userContextCallback
);
```

## Parameters
* `iotHubClientHandle` The handle created by a call to the create function. 

* `reportedState` The current device property values to be 'reported' to the IoTHub. 

* `reportedStateCallback` The callback specified by the device client to be called with the result of the transaction. 

* `userContextCallback` User specified context that will be provided to the callback. This can be NULL.

**NOTE:** The application behavior is undefined if the user calls the [IoTHubClient_LL_Destroy](../iot-c-ref-iothub-client-ll-h/iothubclient-ll-destroy.md) function from within any callback.

## Return Value
IOTHUB_CLIENT_OK upon success or an error code upon failure.

