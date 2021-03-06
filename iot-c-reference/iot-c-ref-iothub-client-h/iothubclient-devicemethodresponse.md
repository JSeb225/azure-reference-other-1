# IoTHubClient_DeviceMethodResponse()

This API responses to a asnyc method callback identified the methodId.

## Syntax

\#include "[azure-iot-sdk-c/iothub_client/inc/iothub_client.h](../iot-c-ref-iothub-client-h.md)"  
```C
IOTHUB_CLIENT_RESULT IoTHubClient_DeviceMethodResponse(
  IOTHUB_CLIENT_HANDLE   iotHubClientHandle,
  METHOD_HANDLE          methodId,
  const unsigned char *  response,
  size_t                 response_size,
  int                    statusCode
);
```

## Parameters
* `iotHubClientHandle` The handle created by a call to the create function. 

* `methodId` The methodId of the Device Method callback. 

* `response` The response data for the method callback. 

* `response_size` The size of the response data buffer. 

* `status_response` The status response of the method callback.

## Return Value
IOTHUB_CLIENT_OK upon success or an error code upon failure.

