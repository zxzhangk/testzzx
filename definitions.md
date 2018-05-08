
<a name="paths"></a>
## Resources

<a name="access-entry-controller_resource"></a>
### Access-entry-controller
Access Entry Controller


<a name="createaccessentryusingpost"></a>
#### createAccessEntry
```
POST /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**accessEntryDTO**  <br>*required*|accessEntryDTO|[AccessEntryDTO](#accessentrydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AccessEntryDTO»](#e0a4cca5f895bff417903983cf01fd30)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pagelistusingget"></a>
#### pageList
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AccessEntryDTO»](#55b745a6916d53fca0142a3882e261f7)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="checkaccessentrynameuniqueusingget"></a>
#### checkAccessEntryNameUnique
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/check-name
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**id**  <br>*optional*|id|integer(int64)|
|**Query**|**name**  <br>*required*|name|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«boolean»](#672f20f336fc0364c54edbe0377bad32)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="idsusingget"></a>
#### ids
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/ids
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**ids**  <br>*required*|ids|< integer(int64) > array(multi)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AccessEntryDTO»»](#f287f3f0903f4d25e72d26aee0007d68)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getuniqueportusingget"></a>
#### getUniquePort
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/ports
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«long»](#3c7c196cd85f782e0dfbb179caf96625)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getusingget"></a>
#### get
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/{accessId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**accessId**  <br>*required*|accessId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AccessEntryDTO»](#e0a4cca5f895bff417903983cf01fd30)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateusingput"></a>
#### update
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/{accessId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**accessId**  <br>*required*|accessId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**accessEntryDTO**  <br>*required*|accessEntryDTO|[AccessEntryDTO](#accessentrydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="deleteusingdelete"></a>
#### delete
```
DELETE /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/{accessId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**accessId**  <br>*required*|accessId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AccessEntryDTO»](#e0a4cca5f895bff417903983cf01fd30)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="bindusingput"></a>
#### bind
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/{accessId}/bind/{servicePortId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**accessId**  <br>*required*|accessId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**servicePortId**  <br>*required*|servicePortId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**accessEntryDTO**  <br>*required*|accessEntryDTO|[AccessEntryDTO](#accessentrydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AccessEntryDTO»](#e0a4cca5f895bff417903983cf01fd30)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="unbindusingput"></a>
#### unbind
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/accesses/{accessId}/unbind
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**accessId**  <br>*required*|accessId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AccessEntryDTO»](#e0a4cca5f895bff417903983cf01fd30)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="alarm-record-admin-controller_resource"></a>
### Alarm-record-admin-controller
Alarm Record Admin Controller


<a name="createalarmrecordusingpost"></a>
#### createAlarmRecord
```
POST /api/v1/admin/alarm-records
```


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|No Content|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listusingget"></a>
#### list
```
GET /api/v1/admin/alarm-records
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AlarmRecordDTO»](#57e4c9dbaddbe91c1155f626bb4c59f4)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="alarm-record-controller_resource"></a>
### Alarm-record-controller
Alarm Record Controller


<a name="listusingget_1"></a>
#### list
```
GET /api/v1/tenants/{tenantId}/alarm-records
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AlarmRecordDTO»](#57e4c9dbaddbe91c1155f626bb4c59f4)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="alarm-strategy-controller_resource"></a>
### Alarm-strategy-controller
Alarm Strategy Controller


<a name="createusingpost"></a>
#### create
```
POST /api/v1/tenants/{tenantId}/alarm-strategies
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**alarmStrategy**  <br>*required*|alarmStrategy|[AlarmStrategyDTO](#alarmstrategydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AlarmStrategyDTO»](#820e429ba436646d1ba3511cdb8e46e4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listusingget_2"></a>
#### list
```
GET /api/v1/tenants/{tenantId}/alarm-strategies
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AlarmStrategyItemDTO»](#5beb6f315d500b9ff325506700a53ec4)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="validatealarmstrategynameusingget"></a>
#### validateAlarmStrategyName
```
GET /api/v1/tenants/{tenantId}/alarm-strategies/duplication-name
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**name**  <br>*required*|name|string|
|**Query**|**oid**  <br>*optional*|oid|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«boolean»](#672f20f336fc0364c54edbe0377bad32)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="deletealarmstrategyusingdelete"></a>
#### deleteAlarmStrategy
```
DELETE /api/v1/tenants/{tenantId}/alarm-strategies/{alarmStrategyId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**alarmStrategyId**  <br>*required*|alarmStrategyId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getusingget_1"></a>
#### get
```
GET /api/v1/tenants/{tenantId}/alarm-strategies/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AlarmStrategyDTO»](#820e429ba436646d1ba3511cdb8e46e4)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateusingput_1"></a>
#### update
```
PUT /api/v1/tenants/{tenantId}/alarm-strategies/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**alarmStrategyNameDTO**  <br>*required*|alarmStrategyNameDTO|[AlarmStrategyNameDTO](#alarmstrategynamedto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AlarmStrategyDTO»](#820e429ba436646d1ba3511cdb8e46e4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updatealarmrulelistusingput"></a>
#### updateAlarmRuleList
```
PUT /api/v1/tenants/{tenantId}/alarm-strategies/{id}/alarm-rules
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**alarmRuleListDTO**  <br>*required*|alarmRuleListDTO|[AlarmRuleListDTO](#alarmrulelistdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AlarmRuleDTO»»](#5fe717aad570d1d0f7490be81b8e1986)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getalarmnotificationuserlistusingget"></a>
#### getAlarmNotificationUserList
```
GET /api/v1/tenants/{tenantId}/alarm-strategies/{id}/notification-user-list
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AlarmNotificationUserDTO»»](#c0deb390ccd6756e1da6b8ff4db5e7ff)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updatenotificationuserslistusingput"></a>
#### updateNotificationUsersList
```
PUT /api/v1/tenants/{tenantId}/alarm-strategies/{id}/notification-users
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**alarmNotificationUserListDTO**  <br>*required*|alarmNotificationUserListDTO|[AlarmNotificationUserListDTO](#alarmnotificationuserlistdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AlarmNotificationUserDTO»»](#c0deb390ccd6756e1da6b8ff4db5e7ff)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getalarmresourcebindinglistusingget"></a>
#### getAlarmResourceBindingList
```
GET /api/v1/tenants/{tenantId}/alarm-strategies/{id}/resource-binding-list
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AlarmResourceBindingDTO»»](#69526be1f7703a8db67ff528b986db6d)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updatealarmresourcebindingslistusingput"></a>
#### updateAlarmResourceBindingsList
```
PUT /api/v1/tenants/{tenantId}/alarm-strategies/{id}/resource-bindings
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**alarmResourceBindingListDTO**  <br>*required*|alarmResourceBindingListDTO|[AlarmResourceBindingListDTO](#alarmresourcebindinglistdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AlarmResourceBindingDTO»»](#69526be1f7703a8db67ff528b986db6d)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getalarmrulelistusingget"></a>
#### getAlarmRuleList
```
GET /api/v1/tenants/{tenantId}/alarm-strategies/{id}/rule-list
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AlarmRuleDTO»»](#5fe717aad570d1d0f7490be81b8e1986)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="app-blue-green-upgrade-controller_resource"></a>
### App-blue-green-upgrade-controller
App Blue Green Upgrade Controller


<a name="bluegreenupgradeapplicationusingpost"></a>
#### blueGreenUpgradeApplication
```
POST /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{currentAppId}/blue-green-upgrade
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**currentAppId**  <br>*required*|currentAppId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**buBlueGreenDeployDTO**  <br>*required*|buBlueGreenDeployDTO|[BlueGreenDeployDTO](#bluegreendeploydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="app-blue-green-upgrade-task-controller_resource"></a>
### App-blue-green-upgrade-task-controller
App Blue Green Upgrade Task Controller


<a name="pagelistusingget_1"></a>
#### pageList
```
GET /api/v1/tenants/{tenantId}/app-blue-green-upgrade-tasks
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppBlueGreenUpgradeTaskDTO»](#cf49f018aebd710d276489cf12327cb8)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="finishedbluegreenupgradeusingpost"></a>
#### finishedBlueGreenUpgrade
```
POST /api/v1/tenants/{tenantId}/app-blue-green-upgrade-tasks/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppBlueGreenUpgradeTaskDTO»](#f27dbd000d587c56a2226e29bd0e061c)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getusingget_2"></a>
#### get
```
GET /api/v1/tenants/{tenantId}/app-blue-green-upgrade-tasks/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppBlueGreenUpgradeTaskDTO»](#f27dbd000d587c56a2226e29bd0e061c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="cancelbluegreenupgradeusingdelete"></a>
#### cancelBlueGreenUpgrade
```
DELETE /api/v1/tenants/{tenantId}/app-blue-green-upgrade-tasks/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppBlueGreenUpgradeTaskDTO»](#f27dbd000d587c56a2226e29bd0e061c)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="toggledefaultaccessappusingput"></a>
#### toggleDefaultAccessApp
```
PUT /api/v1/tenants/{tenantId}/app-blue-green-upgrade-tasks/{id}/{defaultAccessAppId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*required*|userId|string|
|**Path**|**defaultAccessAppId**  <br>*required*|defaultAccessAppId|integer(int64)|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="application-admin-controller_resource"></a>
### Application-admin-controller
Application Admin Controller


<a name="listusingget_3"></a>
#### list
```
GET /api/v1/admin/apps
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppDTO»](#e473848ad49dda7f753aa9d9a46b633d)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappstatisticbynamespaceusingget"></a>
#### getAppStatisticByNamespace
```
GET /api/v1/admin/apps/namespace-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppStatisticDTO»](#ff7fcafaa2850fd9884f92b492c6a2d2)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappquantitystatisticlistusingget"></a>
#### getAppQuantityStatisticList
```
GET /api/v1/admin/apps/quantity
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Query**|**namespace**  <br>*optional*|namespace|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AllQuantityStatisticDTO»](#5515a87bab5e262eb517263a65c34586)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappstatuslistusingget"></a>
#### getAppStatusList
```
GET /api/v1/admin/apps/status-list
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Query**|**namespace**  <br>*optional*|namespace|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AppStatusDTO»»](#f60e221ad6989af4e844fdd31f39f24c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappstatisticbytenantusingget"></a>
#### getAppStatisticByTenant
```
GET /api/v1/admin/apps/tenant-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppStatisticDTO»](#ff7fcafaa2850fd9884f92b492c6a2d2)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getusingget_3"></a>
#### get
```
GET /api/v1/admin/apps/{appId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateusingput_2"></a>
#### update
```
PUT /api/v1/admin/apps/{appId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Body**|**appDTO**  <br>*required*|appDTO|[AppDTO](#appdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="application-controller_resource"></a>
### Application-controller
Operations about apps


<a name="listusingget_4"></a>
#### list
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppDTO»](#e473848ad49dda7f753aa9d9a46b633d)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="checknamespacenameusingget"></a>
#### checkNamespaceName
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/duplication-name
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**appId**  <br>*optional*|appId|integer(int64)|
|**Query**|**appName**  <br>*required*|appName|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«boolean»](#672f20f336fc0364c54edbe0377bad32)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getusingget_4"></a>
#### Find app by appId
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}
```


##### Description
Returns a app when ID < 10. ID > 10 or nonintegers will simulate API error conditions


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseEntity](#responseentity)|
|**400**|Invalid appId supplied|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|App not found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateusingput_3"></a>
#### update
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**appDTO**  <br>*required*|appDTO|[AppDTO](#appdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="canceltopusingput"></a>
#### cancelTop
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}/cancel-top
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="redeployusingput"></a>
#### redeploy
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}/redeploy
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="servicesusingget"></a>
#### services
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}/services
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ServiceDTO»](#ea04e2b28f47862195db8fe73dfea73c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="startusingput"></a>
#### start
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}/start
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="stopusingput"></a>
#### stop
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}/stop
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="topusingput"></a>
#### top
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{appId}/top
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**appId**  <br>*required*|appId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="deleteapplicationusingdelete"></a>
#### deleteApplication
```
DELETE /api/v1/tenants/{tenantId}/namespaces/{namespace}/apps/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="application-create-controller_resource"></a>
### Application-create-controller
Application Create Controller


<a name="createapplicationusingpost"></a>
#### createApplication
```
POST /api/v1/tenants/{tenantId}/apps
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**appDTO**  <br>*required*|appDTO|[AppDTO](#appdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AppDTO»](#6d4188017546b61e6f1534c261439d31)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="application-statistics-controller_resource"></a>
### Application-statistics-controller
Application Statistics Controller


<a name="blueprintappandpodstatisticsusingget"></a>
#### blueprintAppAndPodStatistics
```
GET /api/v1/tenants/{tenantId}/apps/blueprint-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«BlueprintAppStatisticsDTO»»](#366a8845096a0c0fd156d4accfe4031d)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getbuleprintversionappservicepodcpumemcountusingget"></a>
#### getBuleprintVersionAppServicePodCpuMemCount
```
GET /api/v1/tenants/{tenantId}/apps/blueprint-version-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«BlueprintVersionAppStatisticsDTO»](#47bbc53bafe1292d239c21f2ebefc0f6)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappstatisticbynamespaceusingget_1"></a>
#### getAppStatisticByNamespace
```
GET /api/v1/tenants/{tenantId}/apps/namespace-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppStatisticDTO»](#ff7fcafaa2850fd9884f92b492c6a2d2)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappquantitystatisticlistusingget_1"></a>
#### getAppQuantityStatisticList
```
GET /api/v1/tenants/{tenantId}/apps/quantity
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**namespace**  <br>*optional*|namespace|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«AllQuantityStatisticDTO»](#5515a87bab5e262eb517263a65c34586)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappstatuslistusingget_1"></a>
#### getAppStatusList
```
GET /api/v1/tenants/{tenantId}/apps/status-list
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**namespace**  <br>*optional*|namespace|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«AppStatusDTO»»](#f60e221ad6989af4e844fdd31f39f24c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getappstatisticbytenantusingget_1"></a>
#### getAppStatisticByTenant
```
GET /api/v1/tenants/{tenantId}/apps/tenant-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«AppStatisticDTO»](#ff7fcafaa2850fd9884f92b492c6a2d2)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="config-file-controller_resource"></a>
### Config-file-controller
Config File Controller


<a name="createusingpost_1"></a>
#### create
```
POST /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-files
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**configFileDTO**  <br>*required*|configFileDTO|[ConfigFileDTO](#configfiledto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ConfigFileDTO»](#57f4509331e611078109ae26b99216f3)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="validateduplicateconfigfilenameusingget"></a>
#### validateDuplicateConfigFileName
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-files/validate/{configGroupOid}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**configGroupOid**  <br>*required*|configGroupOid|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**name**  <br>*required*|name|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«boolean»](#672f20f336fc0364c54edbe0377bad32)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateusingput_4"></a>
#### update
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-files/{configFileOid}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**configFileOid**  <br>*required*|configFileOid|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**configFileDTO**  <br>*required*|configFileDTO|[ConfigFileDTO](#configfiledto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ConfigFileDTO»](#57f4509331e611078109ae26b99216f3)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="deleteusingdelete_1"></a>
#### delete
```
DELETE /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-files/{configFileOid}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**configFileOid**  <br>*required*|configFileOid|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ConfigFileDTO»](#57f4509331e611078109ae26b99216f3)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listusingget_5"></a>
#### list
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-files/{configGroupOid}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**configGroupOid**  <br>*required*|configGroupOid|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ConfigFileDTO»](#9a9af1e990c0e11efdaf10ebd8034803)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="config-group-controller_resource"></a>
### Config-group-controller
Config Group Controller


<a name="createusingpost_2"></a>
#### create
```
POST /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**configGroupDTO**  <br>*required*|configGroupDTO|[ConfigGroupDTO](#configgroupdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ConfigGroupDTO»](#36a270ec729770c3f5637a1656c345f1)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listusingget_6"></a>
#### list
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ConfigGroupDTO»](#df0fe62af71397bf3bd19c397a2a519b)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="validateduplicateconfiggroupnameusingget"></a>
#### validateDuplicateConfigGroupName
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups/duplication-name
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**name**  <br>*required*|name|string|
|**Query**|**oid**  <br>*optional*|oid|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«boolean»](#672f20f336fc0364c54edbe0377bad32)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listconfiggroupusingget"></a>
#### listConfigGroup
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups/list
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ConfigGroupDTO»](#df0fe62af71397bf3bd19c397a2a519b)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listconfigfilesbyserviceidsusingget"></a>
#### listConfigFilesByServiceIds
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups/services
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**serviceIds**  <br>*required*|serviceIds|< integer(int64) > array(multi)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«List«ServiceMountConfigDTO»»](#408628c25664ae0424d457f0e92815f8)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateusingput_5"></a>
#### update
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups/{configGroupOid}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**configGroupOid**  <br>*required*|configGroupOid|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**configGroupDTO**  <br>*required*|configGroupDTO|[ConfigGroupDTO](#configgroupdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ConfigGroupDTO»](#36a270ec729770c3f5637a1656c345f1)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="deleteusingdelete_2"></a>
#### delete
```
DELETE /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups/{configGroupOid}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**configGroupOid**  <br>*required*|configGroupOid|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ConfigGroupDTO»](#36a270ec729770c3f5637a1656c345f1)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="listconfigfilesbyserviceidusingget"></a>
#### listConfigFilesByServiceId
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/config-groups/{serviceId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceMountConfigDTO»](#3a7961c86fc7d9abf4d4346a70403174)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="config-group-unbind-blueprint-controller_resource"></a>
### Config-group-unbind-blueprint-controller
Config Group Unbind Blueprint Controller


<a name="unbindusingput_1"></a>
#### unbind
```
PUT /api/v1/tenants/{tenantId}/config-groups
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**blueprintVersionList**  <br>*required*|blueprintVersionList|< [BlueprintVersionItem](#blueprintversionitem) > array|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ConfigGroupDTO»](#df0fe62af71397bf3bd19c397a2a519b)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-configuration-admin-controller_resource"></a>
### Pod-configuration-admin-controller
Pod Configuration Admin Controller


<a name="getpodconfigurationusingpost"></a>
#### getPodConfiguration
```
POST /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodconfigurationusingget"></a>
#### getPodConfiguration
```
GET /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodconfigurationusingput"></a>
#### getPodConfiguration
```
PUT /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodconfigurationusingdelete"></a>
#### getPodConfiguration
```
DELETE /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodconfigurationusingpatch"></a>
#### getPodConfiguration
```
PATCH /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodconfigurationusinghead"></a>
#### getPodConfiguration
```
HEAD /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodconfigurationusingoptions"></a>
#### getPodConfiguration
```
OPTIONS /api/v1/admin/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-configuration-controller_resource"></a>
### Pod-configuration-controller
Pod Configuration Controller


<a name="getpodconfigurationusingget_1"></a>
#### getPodConfiguration
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/{id}/configuration
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-controller_resource"></a>
### Pod-controller
Pod Controller


<a name="listpodusingget"></a>
#### listPod
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**query**  <br>*optional*|query|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«PodListDTO»](#3377ee0e976714ec2b18070460941552)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getistiosystemusedinfousingget"></a>
#### getIstioSystemUsedInfo
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/istio-system-used-info
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getpodinfousingget"></a>
#### getPodInfo
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/{podId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**podId**  <br>*required*|podId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="rebuildusingput"></a>
#### rebuild
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/{podId}/rebuild
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**podId**  <br>*required*|podId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«PodDTO»](#e4b229ecfad54776601afec2e5683989)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-logging-admin-controller_resource"></a>
### Pod-logging-admin-controller
Pod Logging Admin Controller


<a name="getpodlogusingget"></a>
#### getPodLog
```
GET /api/v1/admin/pods/{id}/logging
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Query**|**podId**  <br>*optional*||integer(int64)|
|**Query**|**podNameSpace**  <br>*optional*||string|
|**Query**|**uuId**  <br>*optional*||string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[SseEmitter](#sseemitter)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-logging-controller_resource"></a>
### Pod-logging-controller
Pod Logging Controller


<a name="getpodlogusingget_1"></a>
#### getPodLog
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/{id}/logging
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**podId**  <br>*optional*||integer(int64)|
|**Query**|**podNameSpace**  <br>*optional*||string|
|**Query**|**uuId**  <br>*optional*||string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[SseEmitter](#sseemitter)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="heartbeatusingput"></a>
#### heartbeat
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/{id}/logging/heartbeat
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**podId**  <br>*required*|podId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«string»](#a64f53a3c6794c0c188880f3fcf243f9)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-process-admin-controller_resource"></a>
### Pod-process-admin-controller
Pod Process Admin Controller


<a name="createpodprocessdetailwatcherusingget"></a>
#### createPodProcessDetailWatcher
```
GET /api/v1/admin/pods/{id}/process
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**namespace**  <br>*required*|namespace|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="pod-process-controller_resource"></a>
### Pod-process-controller
Pod Process Controller


<a name="createpodprocessdetailwatcherusingget_1"></a>
#### createPodProcessDetailWatcher
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/pods/{id}/process
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|object|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="resource-statistics-admin-controller_resource"></a>
### Resource-statistics-admin-controller
Resource Statistics Admin Controller


<a name="getresourcestatisticsusingget"></a>
#### getResourceStatistics
```
GET /api/v1/admin/resources
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ResourceStatisticsDTO»](#3def45f6b35dceae542dcbe362572a69)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="service-admin-controller_resource"></a>
### Service-admin-controller
Service Admin Controller


<a name="listusingget_7"></a>
#### list
```
GET /api/v1/admin/services
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ServiceDTO»](#ea04e2b28f47862195db8fe73dfea73c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="service-controller_resource"></a>
### Service-controller
Service Controller


<a name="listusingget_8"></a>
#### list
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ServiceDTO»](#ea04e2b28f47862195db8fe73dfea73c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getaccessstatisticsusingget"></a>
#### getAccessStatistics
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/access-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«Map«long,ServiceDTO»»](#eeca704b63e3bea35b4b900dc70b55e5)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="checkservicenameuniqueusingget"></a>
#### checkServiceNameUnique
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/duplication-name
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Query**|**serviceName**  <br>*required*|serviceName|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«boolean»](#672f20f336fc0364c54edbe0377bad32)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getvolumestatisticsusingget"></a>
#### getVolumeStatistics
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/volume-statistics
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«Map«long,List«long»»»](#e47c5f2a1cb0f295b6732fb36d47e48a)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getusingget_5"></a>
#### get
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getnetworksecurityusingget"></a>
#### getNetworkSecurity
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}/network-security
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«NetworkSecurityDTO»](#c9d60ed4836426e80207164ee839e9b9)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="createnetworksecurityusingput"></a>
#### createNetworkSecurity
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}/network-security
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**networkSecurity**  <br>*required*|networkSecurity|[NetworkSecurityDTO](#networksecuritydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="redeployusingput_1"></a>
#### redeploy
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}/redeploy
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="scaleoutusingput"></a>
#### scaleOut
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}/scale-out
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**dto**  <br>*required*|dto|[ServiceScaleOutActionDTO](#servicescaleoutactiondto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="startusingput_1"></a>
#### start
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}/start
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="stopusingput_1"></a>
#### stop
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{id}/stop
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**id**  <br>*required*|id|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="postautoacaleusingpost"></a>
#### postAutoAcale
```
POST /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/auto-scale
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**serviceAutoScaleDTO**  <br>*required*|serviceAutoScaleDTO|[ServiceAutoScaleDTO](#serviceautoscaledto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceAutoScaleDTO»](#94faa3f7759742987ed6a436cc26c11c)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="putautoacaleusingput"></a>
#### putAutoAcale
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/auto-scale
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**serviceAutoScaleDTO**  <br>*required*|serviceAutoScaleDTO|[ServiceAutoScaleDTO](#serviceautoscaledto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceAutoScaleDTO»](#94faa3f7759742987ed6a436cc26c11c)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="autoacalestopusingdelete"></a>
#### autoAcaleStop
```
DELETE /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/auto-scale
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceAutoScaleDTO»](#94faa3f7759742987ed6a436cc26c11c)|
|**204**|No Content|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="getautoacaleusingget"></a>
#### getAutoAcale
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/auto-scale/{autoScaleId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**autoScaleId**  <br>*required*|autoScaleId|integer(int64)|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceAutoScaleDTO»](#94faa3f7759742987ed6a436cc26c11c)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="greyupgradeusingput"></a>
#### greyUpgrade
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/gated-launch
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**serviceDTO**  <br>*required*|serviceDTO|[ServiceDTO](#servicedto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="rollingupgradeusingput"></a>
#### rollingUpgrade
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/rolling-upgrade
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**service**  <br>*required*|service|[ServiceDTO](#servicedto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="scaleupusingput"></a>
#### scaleUp
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/services/{serviceId}/scale-up
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceId**  <br>*required*|serviceId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**scaleUp**  <br>*required*|scaleUp|[ServiceScaleUpDTO](#servicescaleupdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceDTO»](#9083d616ada6e6aa1cee290b61f6deb4)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="service-gray-upgrade-controller_resource"></a>
### Service-gray-upgrade-controller
Service Gray Upgrade Controller


<a name="serviceupgradebyconditionusingget"></a>
#### serviceUpgradeByCondition
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/service-gray-upgrade-tasks
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseEntity](#responseentity)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="serviceupgradebyidusingget"></a>
#### serviceUpgradeById
```
GET /api/v1/tenants/{tenantId}/namespaces/{namespace}/service-gray-upgrade-tasks/{serviceUpgradeId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceUpgradeId**  <br>*required*|serviceUpgradeId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseEntity](#responseentity)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="updateupgradeconfigusingput"></a>
#### updateUpgradeConfig
```
PUT /api/v1/tenants/{tenantId}/namespaces/{namespace}/service-gray-upgrade-tasks/{serviceUpgradeId}
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**namespace**  <br>*required*|namespace|string|
|**Path**|**serviceUpgradeId**  <br>*required*|serviceUpgradeId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**configData**  <br>*required*|configData|[ServiceGrayUpgradeConfigDTO](#servicegrayupgradeconfigdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceGrayUpgradeTaskDTO»](#d5349fb26cca14d78496b40411472aad)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="service-grey-upgrade-action-controller_resource"></a>
### Service-grey-upgrade-action-controller
Service Grey Upgrade Action Controller


<a name="grayscaletoupgradecancelusingput"></a>
#### grayScaleToUpgradeCancel
```
PUT /api/v1/tenants/{tenantId}/services/gated-launch/{launchId}/cancel
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**launchId**  <br>*required*|launchId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceGrayUpgradeTaskDTO»](#d5349fb26cca14d78496b40411472aad)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="grayscaletoupgradefinishusingput"></a>
#### grayScaleToUpgradeFinish
```
PUT /api/v1/tenants/{tenantId}/services/gated-launch/{launchId}/finish
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Header**|**userId**  <br>*optional*|userId|string|
|**Path**|**launchId**  <br>*required*|launchId|integer(int64)|
|**Path**|**tenantId**  <br>*required*|tenantId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«ServiceGrayUpgradeTaskDTO»](#d5349fb26cca14d78496b40411472aad)|
|**201**|Created|No Content|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="service-statistics-controller_resource"></a>
### Service-statistics-controller
Service Statistics Controller


<a name="getserviceusagetop5usingget"></a>
#### getServiceUsageTop5
```
GET /api/v1/tenants/{tenantId}/services/usage
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseList«ServiceUsageDTO»](#0f35c3a4a70af302662528e56e519afb)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`


<a name="volume-monitor-controller_resource"></a>
### Volume-monitor-controller
Volume Monitor Controller


<a name="rangequeryusingget"></a>
#### rangeQuery
```
GET /api/v1/tenants/{tenantId}/volumes/{volumeId}/monitor/series
```


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**tenantId**  <br>*required*|tenantId|string|
|**Path**|**volumeId**  <br>*required*|volumeId|integer(int64)|
|**Body**|**metadata**  <br>*optional*|metadata|[Metadata](#metadata)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[ResponseObject«MonitorResult»](#33de9e2d822c66e885b8c334bbb7e0f4)|
|**401**|Unauthorized|No Content|
|**403**|Forbidden|No Content|
|**404**|Not Found|No Content|


##### Consumes

* `application/json`


##### Produces

* `*/*`







<a name="definitions"></a>
## Definitions

<a name="accessentrydo"></a>
### AccessEntryDO

|Name|Schema|
|---|---|
|**accessType**  <br>*optional*|enum (HTTP, TCP, DOMAIN, IP)|
|**accessUrl**  <br>*optional*|string|
|**appName**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**httpMaxConnection**  <br>*optional*|integer(int32)|
|**httpMaxRequestPerSecond**  <br>*optional*|integer(int32)|
|**httpPath**  <br>*optional*|string|
|**httpRewritePolicy**  <br>*optional*|string|
|**httpSecondLevelDomain**  <br>*optional*|string|
|**httpTopLevelDomain**  <br>*optional*|string|
|**ipAddress**  <br>*optional*|string|
|**ipPort**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**protocol**  <br>*optional*|enum (HTTP, TCP, DOMAIN, IP)|
|**serviceList**  <br>*optional*|< [ServiceListDO](#servicelistdo) > array|
|**serviceName**  <br>*optional*|string|
|**servicePortId**  <br>*optional*|integer(int64)|
|**tenantId**  <br>*optional*|string|


<a name="accessentrydto"></a>
### AccessEntryDTO

|Name|Schema|
|---|---|
|**accessType**  <br>*optional*|enum (HTTP, TCP, DOMAIN, IP)|
|**accessUrl**  <br>*optional*|string|
|**appName**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**httpMaxConnection**  <br>*optional*|integer(int32)|
|**httpMaxRequestPerSecond**  <br>*optional*|integer(int32)|
|**httpPath**  <br>*optional*|string|
|**httpRewritePolicy**  <br>*optional*|string|
|**httpSecondLevelDomain**  <br>*optional*|string|
|**httpTopLevelDomain**  <br>*optional*|string|
|**ipAddress**  <br>*optional*|string|
|**ipPort**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**protocol**  <br>*optional*|enum (HTTP, TCP, DOMAIN, IP)|
|**serviceList**  <br>*optional*|< [ServiceDTO](#servicedto) > array|
|**serviceName**  <br>*optional*|string|
|**servicePortId**  <br>*optional*|integer(int64)|
|**tenantId**  <br>*optional*|string|


<a name="alarmnotificationuserdto"></a>
### AlarmNotificationUserDTO

|Name|Schema|
|---|---|
|**alarmStrategyId**  <br>*optional*|integer(int64)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**notificationUserId**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|


<a name="alarmnotificationuserlistdto"></a>
### AlarmNotificationUserListDTO

|Name|Schema|
|---|---|
|**alarmNotificationUserList**  <br>*required*|< [AlarmNotificationUserDTO](#alarmnotificationuserdto) > array|


<a name="alarmrecorddto"></a>
### AlarmRecordDTO

|Name|Schema|
|---|---|
|**alarmMessage**  <br>*optional*|string|
|**alarmRuleId**  <br>*optional*|integer(int64)|
|**alarmStrategyId**  <br>*optional*|integer(int64)|
|**alarmStrategyName**  <br>*optional*|string|
|**alarmStrategyType**  <br>*optional*|enum (SERVICE, STORAGE_VOLUME)|
|**appName**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**serviceId**  <br>*optional*|integer(int64)|
|**serviceName**  <br>*optional*|string|
|**tenantId**  <br>*optional*|string|
|**volumeId**  <br>*optional*|integer(int64)|
|**volumeName**  <br>*optional*|string|


<a name="alarmresourcebindingdto"></a>
### AlarmResourceBindingDTO

|Name|Schema|
|---|---|
|**alarmStrategyId**  <br>*optional*|integer(int64)|
|**appId**  <br>*optional*|integer(int64)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**pvcName**  <br>*optional*|string|
|**resourceId**  <br>*optional*|integer(int64)|
|**type**  <br>*optional*|enum (SERVICE, STORAGE_VOLUME)|
|**volumeName**  <br>*optional*|string|


<a name="alarmresourcebindinglistdto"></a>
### AlarmResourceBindingListDTO

|Name|Schema|
|---|---|
|**alarmResourceBindingList**  <br>*required*|< [AlarmResourceBindingDTO](#alarmresourcebindingdto) > array|


<a name="alarmruledto"></a>
### AlarmRuleDTO

|Name|Schema|
|---|---|
|**alarmStrategyId**  <br>*optional*|integer(int64)|
|**alarmTarget**  <br>*optional*|enum (SERVICE_STATUS, POD_CPU_RATE, POD_MEM_RATE, POD_DISK_READ_RATE, POD_DISK_WRITE_RATE, VOLUME_READ_RATE, VOLUME_WRITE_RATE, VOLUME_USAGE)|
|**condition**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**duration**  <br>*optional*|integer(int32)|
|**durationUnit**  <br>*optional*|enum (SECONDS, MINUTES, HOURS, DAYS, WEEKS, YEARS)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**threshold**  <br>*optional*|string|
|**thresholdUnit**  <br>*optional*|enum (PERCENTAGE, KB, MB, GB)|


<a name="alarmrulelistdto"></a>
### AlarmRuleListDTO

|Name|Schema|
|---|---|
|**alarmRuleList**  <br>*required*|< [AlarmRuleDTO](#alarmruledto) > array|


<a name="alarmstrategydto"></a>
### AlarmStrategyDTO

|Name|Schema|
|---|---|
|**alarmNotificationUserList**  <br>*optional*|< [AlarmNotificationUserDTO](#alarmnotificationuserdto) > array|
|**alarmResourceBindingList**  <br>*optional*|< [AlarmResourceBindingDTO](#alarmresourcebindingdto) > array|
|**alarmRuleList**  <br>*optional*|< [AlarmRuleDTO](#alarmruledto) > array|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**type**  <br>*optional*|enum (SERVICE, STORAGE_VOLUME)|


<a name="alarmstrategyitemdto"></a>
### AlarmStrategyItemDTO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**resourceBindingTotal**  <br>*optional*|integer(int32)|
|**resourceType**  <br>*optional*|enum (SERVICE, STORAGE_VOLUME)|
|**ruleTotal**  <br>*optional*|integer(int32)|


<a name="alarmstrategynamedto"></a>
### AlarmStrategyNameDTO

|Name|Schema|
|---|---|
|**name**  <br>*required*|string|


<a name="allquantitystatisticdto"></a>
### AllQuantityStatisticDTO

|Name|Schema|
|---|---|
|**access**  <br>*optional*|< string, integer(int64) > map|
|**app**  <br>*optional*|< string, integer(int64) > map|
|**config**  <br>*optional*|< string, integer(int64) > map|
|**pod**  <br>*optional*|< string, integer(int64) > map|
|**service**  <br>*optional*|< string, integer(int64) > map|


<a name="appbluegreenupgradetaskdto"></a>
### AppBlueGreenUpgradeTaskDTO

|Name|Schema|
|---|---|
|**appName**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**currentApp**  <br>*optional*|[AppDO](#appdo)|
|**currentAppId**  <br>*optional*|integer(int64)|
|**currentAppMainServicePortId**  <br>*optional*|integer(int64)|
|**currentAppWeight**  <br>*optional*|integer(int32)|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**mainAccessId**  <br>*optional*|integer(int64)|
|**namespace**  <br>*optional*|string|
|**newApp**  <br>*optional*|[AppDO](#appdo)|
|**newAppId**  <br>*optional*|integer(int64)|
|**newAppMainServicePortId**  <br>*optional*|integer(int64)|
|**newAppWeight**  <br>*optional*|integer(int32)|
|**oid**  <br>*optional*|integer(int64)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="appdo"></a>
### AppDO

|Name|Schema|
|---|---|
|**accessUrl**  <br>*optional*|string|
|**blueGreenUpgradeFlag**  <br>*optional*|enum (NEW, OLD, IS_UPGRADE, IS_NOT_UPGRADE)|
|**blueprintIcon**  <br>*optional*|string|
|**blueprintId**  <br>*optional*|integer(int64)|
|**blueprintVersionId**  <br>*optional*|integer(int64)|
|**configGroup**  <br>*optional*|[ConfigGroupDO](#configgroupdo)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podCount**  <br>*optional*|integer(int32)|
|**serviceList**  <br>*optional*|< [ServiceDO](#servicedo) > array|
|**serviceRunningCount**  <br>*optional*|integer(int32)|
|**serviceTotalCount**  <br>*optional*|integer(int32)|
|**sortDate**  <br>*optional*|string(date-time)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**taskStatus**  <br>*optional*|enum (STARTING, STOPING, DELETING, REDEPOLYING, UNDER_SCALE_UP, APPLICATION_DEPLOYING, APPLICATION_DELETING, APPLICATION_STARTING, APPLICATION_STOPPING, APPLICATION_REDEPLOYING, SERVICE_DELETING, SERVICE_STARTING, SERVICE_STOPPING, SERVICE_REDEPLOYING, SERVICE_ROLLING_UPGRADING, SERVICE_GRAY_UPGRADING, SERVICE_EXTENDING_HORIZONTAL, SERVICE_EXTENDING_VERTICAL, SERVICE_EXTENDING_ELASTIC, SERVICE_GRAY_UPGRADING_FINISH, SERVICE_GRAY_UPGRADING_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="appdto"></a>
### AppDTO

|Name|Schema|
|---|---|
|**accessUrl**  <br>*optional*|string|
|**blueGreenUpgradeFlag**  <br>*optional*|enum (NEW, OLD, IS_UPGRADE, IS_NOT_UPGRADE)|
|**blueprintIcon**  <br>*optional*|string|
|**blueprintId**  <br>*optional*|integer(int64)|
|**blueprintVersionId**  <br>*optional*|integer(int64)|
|**configGroup**  <br>*optional*|[ConfigGroupDTO](#configgroupdto)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podCount**  <br>*optional*|integer(int32)|
|**serviceList**  <br>*optional*|< [ServiceDTO](#servicedto) > array|
|**serviceRunningCount**  <br>*optional*|integer(int32)|
|**serviceTotalCount**  <br>*optional*|integer(int32)|
|**sortDate**  <br>*optional*|string(date-time)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**taskStatus**  <br>*optional*|enum (STARTING, STOPING, DELETING, REDEPOLYING, UNDER_SCALE_UP, APPLICATION_DEPLOYING, APPLICATION_DELETING, APPLICATION_STARTING, APPLICATION_STOPPING, APPLICATION_REDEPLOYING, SERVICE_DELETING, SERVICE_STARTING, SERVICE_STOPPING, SERVICE_REDEPLOYING, SERVICE_ROLLING_UPGRADING, SERVICE_GRAY_UPGRADING, SERVICE_EXTENDING_HORIZONTAL, SERVICE_EXTENDING_VERTICAL, SERVICE_EXTENDING_ELASTIC, SERVICE_GRAY_UPGRADING_FINISH, SERVICE_GRAY_UPGRADING_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="appstatisticdto"></a>
### AppStatisticDTO

|Name|Schema|
|---|---|
|**appCount**  <br>*optional*|integer(int64)|
|**cpuQuota**  <br>*optional*|integer(int64)|
|**cpuUsage**  <br>*optional*|integer(int64)|
|**memoryQuota**  <br>*optional*|integer(int64)|
|**memoryUsage**  <br>*optional*|integer(int64)|
|**namespace**  <br>*optional*|string|
|**podCount**  <br>*optional*|integer(int64)|
|**podRunning**  <br>*optional*|integer(int64)|
|**tenantId**  <br>*optional*|string|


<a name="appstatusdto"></a>
### AppStatusDTO

|Name|Schema|
|---|---|
|**cpuQuota**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryQuota**  <br>*optional*|integer(int32)|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="bluegreendeploydto"></a>
### BlueGreenDeployDTO

|Name|Schema|
|---|---|
|**accessUrl**  <br>*optional*|string|
|**blueGreenUpgradeFlag**  <br>*optional*|enum (NEW, OLD, IS_UPGRADE, IS_NOT_UPGRADE)|
|**blueprintIcon**  <br>*optional*|string|
|**blueprintId**  <br>*optional*|integer(int64)|
|**blueprintVersionId**  <br>*optional*|integer(int64)|
|**configGroup**  <br>*optional*|[ConfigGroupDTO](#configgroupdto)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**currentAppMainServicePortId**  <br>*optional*|integer(int64)|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**mainAccessId**  <br>*optional*|integer(int64)|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**newAppMainServiceName**  <br>*optional*|string|
|**newAppMainServiceOuterPort**  <br>*optional*|integer(int64)|
|**oid**  <br>*optional*|integer(int64)|
|**podCount**  <br>*optional*|integer(int32)|
|**serviceList**  <br>*optional*|< [ServiceDTO](#servicedto) > array|
|**serviceRunningCount**  <br>*optional*|integer(int32)|
|**serviceTotalCount**  <br>*optional*|integer(int32)|
|**sortDate**  <br>*optional*|string(date-time)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**taskStatus**  <br>*optional*|enum (STARTING, STOPING, DELETING, REDEPOLYING, UNDER_SCALE_UP, APPLICATION_DEPLOYING, APPLICATION_DELETING, APPLICATION_STARTING, APPLICATION_STOPPING, APPLICATION_REDEPLOYING, SERVICE_DELETING, SERVICE_STARTING, SERVICE_STOPPING, SERVICE_REDEPLOYING, SERVICE_ROLLING_UPGRADING, SERVICE_GRAY_UPGRADING, SERVICE_EXTENDING_HORIZONTAL, SERVICE_EXTENDING_VERTICAL, SERVICE_EXTENDING_ELASTIC, SERVICE_GRAY_UPGRADING_FINISH, SERVICE_GRAY_UPGRADING_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="blueprintappstatisticsdto"></a>
### BlueprintAppStatisticsDTO

|Name|Schema|
|---|---|
|**appTotal**  <br>*optional*|integer(int64)|
|**blueprintId**  <br>*optional*|integer(int64)|
|**podTotal**  <br>*optional*|integer(int64)|


<a name="blueprintversionappstatisticsdto"></a>
### BlueprintVersionAppStatisticsDTO

|Name|Schema|
|---|---|
|**appTotal**  <br>*optional*|integer(int64)|
|**blueprintVersionId**  <br>*optional*|integer(int64)|
|**cpuQuota**  <br>*optional*|integer(int64)|
|**memoryQuota**  <br>*optional*|integer(int64)|
|**podTotal**  <br>*optional*|integer(int64)|
|**serviceTotal**  <br>*optional*|integer(int64)|


<a name="blueprintversionitem"></a>
### BlueprintVersionItem

|Name|Schema|
|---|---|
|**blueprintOid**  <br>*required*|integer(int64)|
|**blueprintVersionOid**  <br>*required*|integer(int64)|


<a name="configfiledo"></a>
### ConfigFileDO

|Name|Schema|
|---|---|
|**configGroupOid**  <br>*optional*|integer(int64)|
|**content**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**k8sName**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**serviceName**  <br>*optional*|string|
|**tenantId**  <br>*optional*|string|


<a name="configfiledto"></a>
### ConfigFileDTO

|Name|Schema|
|---|---|
|**configGroupOid**  <br>*optional*|integer(int64)|
|**content**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**k8sName**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**serviceName**  <br>*optional*|string|
|**tenantId**  <br>*optional*|string|


<a name="configgroupdo"></a>
### ConfigGroupDO

|Name|Schema|
|---|---|
|**appName**  <br>*optional*|string|
|**blueprintOid**  <br>*optional*|integer(int64)|
|**blueprintVersionOid**  <br>*optional*|integer(int64)|
|**configFileList**  <br>*optional*|< [ConfigFileDO](#configfiledo) > array|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**displayName**  <br>*optional*|string|
|**filesCount**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**tenantId**  <br>*optional*|string|


<a name="configgroupdto"></a>
### ConfigGroupDTO

|Name|Schema|
|---|---|
|**appName**  <br>*optional*|string|
|**blueprintOid**  <br>*optional*|integer(int64)|
|**blueprintVersionOid**  <br>*optional*|integer(int64)|
|**configFileList**  <br>*optional*|< [ConfigFileDTO](#configfiledto) > array|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**description**  <br>*optional*|string|
|**displayName**  <br>*optional*|string|
|**filesCount**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**tenantId**  <br>*optional*|string|


<a name="data"></a>
### Data

|Name|Schema|
|---|---|
|**result**  <br>*optional*|< [Result](#result) > array|
|**resultType**  <br>*optional*|string|


<a name="afac7df0f8c231288052181c72aee852"></a>
### Map«long,List«long»»
*Type* : < string, [List](#list) > map


<a name="b084c67efae5140f90d330bd8c77d156"></a>
### Map«long,ServiceDTO»
*Type* : < string, [ServiceDTO](#servicedto) > map


<a name="metadata"></a>
### Metadata

|Name|Schema|
|---|---|
|**ext**  <br>*optional*|< string > array|
|**filter**  <br>*optional*|< string, string > map|
|**paginationParam**  <br>*optional*|[PaginationParam](#paginationparam)|


<a name="metric"></a>
### Metric

|Name|Schema|
|---|---|
|**__name__**  <br>*optional*|string|
|**build_date**  <br>*optional*|string|
|**container_image**  <br>*optional*|string|
|**container_name**  <br>*optional*|string|
|**container_version**  <br>*optional*|string|
|**cpu**  <br>*optional*|string|
|**domain**  <br>*optional*|string|
|**fstype**  <br>*optional*|string|
|**host**  <br>*optional*|string|
|**instance**  <br>*optional*|string|
|**interface**  <br>*optional*|string|
|**job**  <br>*optional*|string|
|**kolla_version**  <br>*optional*|string|
|**license**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**network**  <br>*optional*|string|
|**path**  <br>*optional*|string|
|**state**  <br>*optional*|string|
|**vendor**  <br>*optional*|string|
|**vm_disk_name**  <br>*optional*|string|
|**vm_mac**  <br>*optional*|string|
|**vm_os**  <br>*optional*|string|
|**vm_uuid**  <br>*optional*|string|
|**vm_vif**  <br>*optional*|string|


<a name="monitorresult"></a>
### MonitorResult

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[Data](#data)|
|**status**  <br>*optional*|string|


<a name="mountconfigdto"></a>
### MountConfigDTO

|Name|Schema|
|---|---|
|**configFileList**  <br>*optional*|< [ConfigFileDTO](#configfiledto) > array|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**path**  <br>*optional*|string|


<a name="networksecuritydto"></a>
### NetworkSecurityDTO

|Name|Schema|
|---|---|
|**accessControl**  <br>*optional*|enum (UNLIMITED, DENY_ALL, SECURITY_POLICY)|
|**policyList**  <br>*optional*|< [SecurityPolicyDTO](#securitypolicydto) > array|


<a name="paginationparam"></a>
### PaginationParam

|Name|Schema|
|---|---|
|**page**  <br>*optional*|integer(int32)|
|**pageSize**  <br>*optional*|integer(int32)|
|**totalCount**  <br>*optional*|integer(int32)|


<a name="poddo"></a>
### PodDO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**innerIp**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**serviceId**  <br>*optional*|integer(int64)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="poddto"></a>
### PodDTO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**innerIp**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**service**  <br>*optional*|[ServiceDTO](#servicedto)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|


<a name="podlistdto"></a>
### PodListDTO

|Name|Schema|
|---|---|
|**appId**  <br>*optional*|integer(int64)|
|**appName**  <br>*optional*|string|
|**appTimeCreated**  <br>*optional*|string(date-time)|
|**blueprintId**  <br>*optional*|integer(int64)|
|**blueprintVersionId**  <br>*optional*|integer(int64)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**icon**  <br>*optional*|string|
|**image**  <br>*optional*|string|
|**imageDomain**  <br>*optional*|string|
|**imageVersion**  <br>*optional*|string|
|**innerIp**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**registry**  <br>*optional*|string|
|**serviceName**  <br>*optional*|string|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|


<a name="resourcestatisticsdto"></a>
### ResourceStatisticsDTO

|Name|Schema|
|---|---|
|**accessCount**  <br>*optional*|integer(int64)|
|**configGroupCount**  <br>*optional*|integer(int64)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|


<a name="responseentity"></a>
### ResponseEntity

|Name|Schema|
|---|---|
|**body**  <br>*optional*|object|
|**statusCode**  <br>*optional*|enum (100, 101, 102, 103, 200, 201, 202, 203, 204, 205, 206, 207, 208, 226, 300, 301, 302, 302, 303, 304, 305, 307, 308, 400, 401, 402, 403, 404, 405, 406, 407, 408, 409, 410, 411, 412, 413, 413, 414, 414, 415, 416, 417, 418, 419, 420, 421, 422, 423, 424, 426, 428, 429, 431, 451, 500, 501, 502, 503, 504, 505, 506, 507, 508, 509, 510, 511)|
|**statusCodeValue**  <br>*optional*|integer(int32)|


<a name="55b745a6916d53fca0142a3882e261f7"></a>
### ResponseList«AccessEntryDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«AccessEntryDTO»](#0072b701c41879cbcd53386f0bc0dd31)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="57e4c9dbaddbe91c1155f626bb4c59f4"></a>
### ResponseList«AlarmRecordDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«AlarmRecordDTO»](#64ecf3eaef936750557119ecaaf5ad2e)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="5beb6f315d500b9ff325506700a53ec4"></a>
### ResponseList«AlarmStrategyItemDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«AlarmStrategyItemDTO»](#cd1c53663c605508f09b06b4024bd5d2)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="cf49f018aebd710d276489cf12327cb8"></a>
### ResponseList«AppBlueGreenUpgradeTaskDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«AppBlueGreenUpgradeTaskDTO»](#cea320b07aec5e99cae3445b598ef188)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="e473848ad49dda7f753aa9d9a46b633d"></a>
### ResponseList«AppDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«AppDTO»](#9eae90142245b03ad87afece4db43235)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="ff7fcafaa2850fd9884f92b492c6a2d2"></a>
### ResponseList«AppStatisticDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«AppStatisticDTO»](#5ffb85cf8624a82f80a789a74f3af74a)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="47bbc53bafe1292d239c21f2ebefc0f6"></a>
### ResponseList«BlueprintVersionAppStatisticsDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«BlueprintVersionAppStatisticsDTO»](#6fcfd8108bba47134fe198975b9f8374)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="9a9af1e990c0e11efdaf10ebd8034803"></a>
### ResponseList«ConfigFileDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«ConfigFileDTO»](#8352c0d588619399dbffc26b7aa98fd8)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="df0fe62af71397bf3bd19c397a2a519b"></a>
### ResponseList«ConfigGroupDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«ConfigGroupDTO»](#096d15096f2457191f8446a93b7cdd06)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="3377ee0e976714ec2b18070460941552"></a>
### ResponseList«PodListDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«PodListDTO»](#e08e507bb172a112c9ae83ead3c8633a)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="ea04e2b28f47862195db8fe73dfea73c"></a>
### ResponseList«ServiceDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«ServiceDTO»](#d4ffb30b5a93fa68799ed3f7aa076d97)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="0f35c3a4a70af302662528e56e519afb"></a>
### ResponseList«ServiceUsageDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResultSet«ServiceUsageDTO»](#498296fe4b6e82524779c557758c1fb8)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="e0a4cca5f895bff417903983cf01fd30"></a>
### ResponseObject«AccessEntryDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[AccessEntryDTO](#accessentrydto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="820e429ba436646d1ba3511cdb8e46e4"></a>
### ResponseObject«AlarmStrategyDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[AlarmStrategyDTO](#alarmstrategydto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="5515a87bab5e262eb517263a65c34586"></a>
### ResponseObject«AllQuantityStatisticDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[AllQuantityStatisticDTO](#allquantitystatisticdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="f27dbd000d587c56a2226e29bd0e061c"></a>
### ResponseObject«AppBlueGreenUpgradeTaskDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[AppBlueGreenUpgradeTaskDTO](#appbluegreenupgradetaskdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="6d4188017546b61e6f1534c261439d31"></a>
### ResponseObject«AppDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[AppDTO](#appdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="57f4509331e611078109ae26b99216f3"></a>
### ResponseObject«ConfigFileDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ConfigFileDTO](#configfiledto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="36a270ec729770c3f5637a1656c345f1"></a>
### ResponseObject«ConfigGroupDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ConfigGroupDTO](#configgroupdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="f287f3f0903f4d25e72d26aee0007d68"></a>
### ResponseObject«List«AccessEntryDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [AccessEntryDTO](#accessentrydto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="c0deb390ccd6756e1da6b8ff4db5e7ff"></a>
### ResponseObject«List«AlarmNotificationUserDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [AlarmNotificationUserDTO](#alarmnotificationuserdto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="69526be1f7703a8db67ff528b986db6d"></a>
### ResponseObject«List«AlarmResourceBindingDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [AlarmResourceBindingDTO](#alarmresourcebindingdto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="5fe717aad570d1d0f7490be81b8e1986"></a>
### ResponseObject«List«AlarmRuleDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [AlarmRuleDTO](#alarmruledto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="f60e221ad6989af4e844fdd31f39f24c"></a>
### ResponseObject«List«AppStatusDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [AppStatusDTO](#appstatusdto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="366a8845096a0c0fd156d4accfe4031d"></a>
### ResponseObject«List«BlueprintAppStatisticsDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [BlueprintAppStatisticsDTO](#blueprintappstatisticsdto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="408628c25664ae0424d457f0e92815f8"></a>
### ResponseObject«List«ServiceMountConfigDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< [ServiceMountConfigDTO](#servicemountconfigdto) > array|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="e47c5f2a1cb0f295b6732fb36d47e48a"></a>
### ResponseObject«Map«long,List«long»»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< string, [List](#list) > map|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="eeca704b63e3bea35b4b900dc70b55e5"></a>
### ResponseObject«Map«long,ServiceDTO»»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|< string, [ServiceDTO](#servicedto) > map|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="33de9e2d822c66e885b8c334bbb7e0f4"></a>
### ResponseObject«MonitorResult»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[MonitorResult](#monitorresult)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="c9d60ed4836426e80207164ee839e9b9"></a>
### ResponseObject«NetworkSecurityDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[NetworkSecurityDTO](#networksecuritydto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="e4b229ecfad54776601afec2e5683989"></a>
### ResponseObject«PodDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[PodDTO](#poddto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="3def45f6b35dceae542dcbe362572a69"></a>
### ResponseObject«ResourceStatisticsDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ResourceStatisticsDTO](#resourcestatisticsdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="94faa3f7759742987ed6a436cc26c11c"></a>
### ResponseObject«ServiceAutoScaleDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ServiceAutoScaleDTO](#serviceautoscaledto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="9083d616ada6e6aa1cee290b61f6deb4"></a>
### ResponseObject«ServiceDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ServiceDTO](#servicedto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="d5349fb26cca14d78496b40411472aad"></a>
### ResponseObject«ServiceGrayUpgradeTaskDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ServiceGrayUpgradeTaskDTO](#servicegrayupgradetaskdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="3a7961c86fc7d9abf4d4346a70403174"></a>
### ResponseObject«ServiceMountConfigDTO»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|[ServiceMountConfigDTO](#servicemountconfigdto)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="672f20f336fc0364c54edbe0377bad32"></a>
### ResponseObject«boolean»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|boolean|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="3c7c196cd85f782e0dfbb179caf96625"></a>
### ResponseObject«long»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|integer(int64)|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="a64f53a3c6794c0c188880f3fcf243f9"></a>
### ResponseObject«string»

|Name|Schema|
|---|---|
|**data**  <br>*optional*|string|
|**errorCode**  <br>*optional*|string|
|**status**  <br>*optional*|integer(int32)|
|**userMessage**  <br>*optional*|string|


<a name="result"></a>
### Result

|Name|Schema|
|---|---|
|**metric**  <br>*optional*|[Metric](#metric)|
|**value**  <br>*optional*|< object > array|
|**values**  <br>*optional*|< < object > array > array|


<a name="0072b701c41879cbcd53386f0bc0dd31"></a>
### ResultSet«AccessEntryDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [AccessEntryDTO](#accessentrydto) > array|


<a name="64ecf3eaef936750557119ecaaf5ad2e"></a>
### ResultSet«AlarmRecordDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [AlarmRecordDTO](#alarmrecorddto) > array|


<a name="cd1c53663c605508f09b06b4024bd5d2"></a>
### ResultSet«AlarmStrategyItemDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [AlarmStrategyItemDTO](#alarmstrategyitemdto) > array|


<a name="cea320b07aec5e99cae3445b598ef188"></a>
### ResultSet«AppBlueGreenUpgradeTaskDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [AppBlueGreenUpgradeTaskDTO](#appbluegreenupgradetaskdto) > array|


<a name="9eae90142245b03ad87afece4db43235"></a>
### ResultSet«AppDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [AppDTO](#appdto) > array|


<a name="5ffb85cf8624a82f80a789a74f3af74a"></a>
### ResultSet«AppStatisticDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [AppStatisticDTO](#appstatisticdto) > array|


<a name="6fcfd8108bba47134fe198975b9f8374"></a>
### ResultSet«BlueprintVersionAppStatisticsDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [BlueprintVersionAppStatisticsDTO](#blueprintversionappstatisticsdto) > array|


<a name="8352c0d588619399dbffc26b7aa98fd8"></a>
### ResultSet«ConfigFileDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [ConfigFileDTO](#configfiledto) > array|


<a name="096d15096f2457191f8446a93b7cdd06"></a>
### ResultSet«ConfigGroupDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [ConfigGroupDTO](#configgroupdto) > array|


<a name="e08e507bb172a112c9ae83ead3c8633a"></a>
### ResultSet«PodListDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [PodListDTO](#podlistdto) > array|


<a name="d4ffb30b5a93fa68799ed3f7aa076d97"></a>
### ResultSet«ServiceDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [ServiceDTO](#servicedto) > array|


<a name="498296fe4b6e82524779c557758c1fb8"></a>
### ResultSet«ServiceUsageDTO»

|Name|Schema|
|---|---|
|**metadata**  <br>*optional*|[Metadata](#metadata)|
|**resultSet**  <br>*optional*|< [ServiceUsageDTO](#serviceusagedto) > array|


<a name="securitypolicydto"></a>
### SecurityPolicyDTO

|Name|Schema|
|---|---|
|**rule**  <br>*required*|enum (ACCESS_IP_RANGE, APPLICATION, ACCESS_PORT)|
|**ruleValue**  <br>*required*|string|


<a name="serviceautoscaledo"></a>
### ServiceAutoScaleDO

|Name|Schema|
|---|---|
|**cpuThreshold**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**enable**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryThreshold**  <br>*optional*|integer(int32)|
|**oid**  <br>*optional*|integer(int64)|
|**podMax**  <br>*optional*|integer(int32)|
|**podMin**  <br>*optional*|integer(int32)|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="serviceautoscaledto"></a>
### ServiceAutoScaleDTO

|Name|Schema|
|---|---|
|**cpuThreshold**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**enable**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryThreshold**  <br>*optional*|integer(int32)|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podMax**  <br>*optional*|integer(int32)|
|**podMin**  <br>*optional*|integer(int32)|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="serviceconfiggroupdo"></a>
### ServiceConfigGroupDO

|Name|Schema|
|---|---|
|**configFileId**  <br>*optional*|integer(int64)|
|**configFileList**  <br>*optional*|< [ConfigFileDO](#configfiledo) > array|
|**configFileName**  <br>*optional*|string|
|**configGroupId**  <br>*optional*|integer(int64)|
|**configGroupName**  <br>*optional*|string|
|**configK8sGroupName**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**path**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="serviceconfiggroupdto"></a>
### ServiceConfigGroupDTO

|Name|Schema|
|---|---|
|**configFileList**  <br>*optional*|< [ConfigFileDTO](#configfiledto) > array|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**path**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="servicedo"></a>
### ServiceDO

|Name|Schema|
|---|---|
|**accessControl**  <br>*optional*|enum (UNLIMITED, DENY_ALL, SECURITY_POLICY)|
|**appId**  <br>*optional*|integer(int64)|
|**configGroup**  <br>*optional*|[ConfigGroupDO](#configgroupdo)|
|**cpuQuota**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**environmentVariable**  <br>*optional*|< string, string > map|
|**icon**  <br>*optional*|string|
|**image**  <br>*optional*|string|
|**imageDomain**  <br>*optional*|string|
|**imageVersion**  <br>*optional*|string|
|**internalIp**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryQuota**  <br>*optional*|integer(int32)|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podList**  <br>*optional*|< [PodDO](#poddo) > array|
|**podRunning**  <br>*optional*|integer(int32)|
|**podTotal**  <br>*optional*|integer(int32)|
|**resourceStatus**  <br>*optional*|< enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL) > array|
|**securityPolicyList**  <br>*optional*|< [ServiceSecurityPolicyDO](#servicesecuritypolicydo) > array|
|**serviceAutoScale**  <br>*optional*|[ServiceAutoScaleDO](#serviceautoscaledo)|
|**serviceConfigGroupList**  <br>*optional*|< [ServiceConfigGroupDO](#serviceconfiggroupdo) > array|
|**serviceEnvironmentList**  <br>*optional*|< [ServiceEnvironmentDO](#serviceenvironmentdo) > array|
|**serviceHealthCheck**  <br>*optional*|[ServiceHealthCheckDO](#servicehealthcheckdo)|
|**servicePortList**  <br>*optional*|< [ServicePortDO](#serviceportdo) > array|
|**serviceVolumeList**  <br>*optional*|< [ServiceVolumeDO](#servicevolumedo) > array|
|**startCommand**  <br>*optional*|string|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**taskStatus**  <br>*optional*|enum (STARTING, STOPING, DELETING, REDEPOLYING, UNDER_SCALE_UP, APPLICATION_DEPLOYING, APPLICATION_DELETING, APPLICATION_STARTING, APPLICATION_STOPPING, APPLICATION_REDEPLOYING, SERVICE_DELETING, SERVICE_STARTING, SERVICE_STOPPING, SERVICE_REDEPLOYING, SERVICE_ROLLING_UPGRADING, SERVICE_GRAY_UPGRADING, SERVICE_EXTENDING_HORIZONTAL, SERVICE_EXTENDING_VERTICAL, SERVICE_EXTENDING_ELASTIC, SERVICE_GRAY_UPGRADING_FINISH, SERVICE_GRAY_UPGRADING_CANCEL)|
|**tenantOid**  <br>*optional*|string|
|**upgradeFlag**  <br>*optional*|enum (NEW, OLD, IS_UPGRADE, IS_NOT_UPGRADE)|
|**useHostTimeZone**  <br>*optional*|boolean|
|**version**  <br>*optional*|integer(int32)|


<a name="servicedto"></a>
### ServiceDTO

|Name|Schema|
|---|---|
|**accessControl**  <br>*optional*|enum (UNLIMITED, DENY_ALL, SECURITY_POLICY)|
|**appId**  <br>*optional*|integer(int64)|
|**appName**  <br>*optional*|string|
|**blueprintId**  <br>*optional*|string|
|**blueprintVersionId**  <br>*optional*|string|
|**configGroup**  <br>*optional*|[ConfigGroupDTO](#configgroupdto)|
|**cpuQuota**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**icon**  <br>*optional*|string|
|**image**  <br>*optional*|string|
|**imageDomain**  <br>*optional*|string|
|**imageVersion**  <br>*optional*|string|
|**internalIp**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryQuota**  <br>*optional*|integer(int32)|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podList**  <br>*optional*|< [PodDTO](#poddto) > array|
|**podRunning**  <br>*optional*|integer(int32)|
|**podTotal**  <br>*optional*|integer(int32)|
|**serviceAutoScale**  <br>*optional*|[ServiceAutoScaleDTO](#serviceautoscaledto)|
|**serviceConfigGroupList**  <br>*optional*|< [ServiceConfigGroupDTO](#serviceconfiggroupdto) > array|
|**serviceEnvironmentList**  <br>*optional*|< [ServiceEnvironmentDTO](#serviceenvironmentdto) > array|
|**serviceHealthCheck**  <br>*optional*|[ServiceHealthCheckDTO](#servicehealthcheckdto)|
|**servicePortList**  <br>*optional*|< [ServicePortDTO](#serviceportdto) > array|
|**serviceVolumeList**  <br>*optional*|< [ServiceVolumeDTO](#servicevolumedto) > array|
|**startCommand**  <br>*optional*|string|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**taskStatus**  <br>*optional*|enum (STARTING, STOPING, DELETING, REDEPOLYING, UNDER_SCALE_UP, APPLICATION_DEPLOYING, APPLICATION_DELETING, APPLICATION_STARTING, APPLICATION_STOPPING, APPLICATION_REDEPLOYING, SERVICE_DELETING, SERVICE_STARTING, SERVICE_STOPPING, SERVICE_REDEPLOYING, SERVICE_ROLLING_UPGRADING, SERVICE_GRAY_UPGRADING, SERVICE_EXTENDING_HORIZONTAL, SERVICE_EXTENDING_VERTICAL, SERVICE_EXTENDING_ELASTIC, SERVICE_GRAY_UPGRADING_FINISH, SERVICE_GRAY_UPGRADING_CANCEL)|
|**tenantOid**  <br>*optional*|string|
|**upgradeFlag**  <br>*optional*|enum (NEW, OLD, IS_UPGRADE, IS_NOT_UPGRADE)|
|**useHostTimeZone**  <br>*optional*|boolean|
|**version**  <br>*optional*|integer(int32)|


<a name="serviceenvironmentdo"></a>
### ServiceEnvironmentDO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**key**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**serviceId**  <br>*optional*|integer(int64)|
|**value**  <br>*optional*|string|


<a name="serviceenvironmentdto"></a>
### ServiceEnvironmentDTO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**key**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**serviceId**  <br>*optional*|integer(int64)|
|**value**  <br>*optional*|string|


<a name="servicegrayupgradeconfigdto"></a>
### ServiceGrayUpgradeConfigDTO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**currentServiceWeight**  <br>*required*|integer(int32)|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**newServiceWeight**  <br>*required*|integer(int32)|
|**oid**  <br>*optional*|integer(int64)|


<a name="servicegrayupgradetaskdto"></a>
### ServiceGrayUpgradeTaskDTO

|Name|Schema|
|---|---|
|**accessIp**  <br>*optional*|string|
|**appId**  <br>*optional*|integer(int64)|
|**appName**  <br>*optional*|string|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**currentService**  <br>*optional*|[ServiceDTO](#servicedto)|
|**currentServiceWeight**  <br>*optional*|integer(int32)|
|**deleted**  <br>*optional*|integer(int32)|
|**domain**  <br>*optional*|string|
|**interalAccessIp**  <br>*optional*|string|
|**interalDomain**  <br>*optional*|string|
|**ipAddress**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**namespaceId**  <br>*optional*|integer(int64)|
|**newService**  <br>*optional*|[ServiceDTO](#servicedto)|
|**newServiceWeight**  <br>*optional*|integer(int32)|
|**oid**  <br>*optional*|integer(int64)|
|**serviceName**  <br>*optional*|string|
|**status**  <br>*optional*|string|
|**statusName**  <br>*optional*|string|
|**tenantId**  <br>*optional*|string|
|**usedTime**  <br>*optional*|integer(int64)|


<a name="servicehealthcheckdo"></a>
### ServiceHealthCheckDO

|Name|Schema|
|---|---|
|**checkInterval**  <br>*optional*|integer(int32)|
|**checkPolicy**  <br>*optional*|enum (HTTP, TCP)|
|**checkTimeout**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**httpUrl**  <br>*optional*|string|
|**initializeTimeout**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**port**  <br>*optional*|integer(int64)|
|**status**  <br>*optional*|enum (ON, OFF)|
|**unhealthThreshold**  <br>*optional*|integer(int32)|


<a name="servicehealthcheckdto"></a>
### ServiceHealthCheckDTO

|Name|Schema|
|---|---|
|**checkInterval**  <br>*optional*|integer(int32)|
|**checkPolicy**  <br>*optional*|enum (HTTP, TCP)|
|**checkTimeout**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**httpUrl**  <br>*optional*|string|
|**initializeTimeout**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**port**  <br>*optional*|integer(int32)|
|**status**  <br>*optional*|enum (ON, OFF)|
|**unhealthThreshold**  <br>*optional*|integer(int32)|


<a name="#servicelistdo"></a>
### ServiceListDO

|Name|Schema|
|---|---|
|**accessControl**  <br>*optional*|enum (UNLIMITED, DENY_ALL, SECURITY_POLICY)|
|**appId**  <br>*optional*|integer(int64)|
|**appName**  <br>*optional*|string|
|**blueprintId**  <br>*optional*|string|
|**blueprintVersionId**  <br>*optional*|string|
|**configGroup**  <br>*optional*|[ConfigGroupDO](#configgroupdo)|
|**cpuQuota**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**environmentVariable**  <br>*optional*|< string, string > map|
|**icon**  <br>*optional*|string|
|**image**  <br>*optional*|string|
|**imageDomain**  <br>*optional*|string|
|**imageVersion**  <br>*optional*|string|
|**internalIp**  <br>*optional*|string|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryQuota**  <br>*optional*|integer(int32)|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podList**  <br>*optional*|< [PodDO](#poddo) > array|
|**podRunning**  <br>*optional*|integer(int32)|
|**podTotal**  <br>*optional*|integer(int32)|
|**resourceStatus**  <br>*optional*|< enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL) > array|
|**securityPolicyList**  <br>*optional*|< [ServiceSecurityPolicyDO](#servicesecuritypolicydo) > array|
|**serviceAutoScale**  <br>*optional*|[ServiceAutoScaleDO](#serviceautoscaledo)|
|**serviceConfigGroupList**  <br>*optional*|< [ServiceConfigGroupDO](#serviceconfiggroupdo) > array|
|**serviceEnvironmentList**  <br>*optional*|< [ServiceEnvironmentDO](#serviceenvironmentdo) > array|
|**serviceHealthCheck**  <br>*optional*|[ServiceHealthCheckDO](#servicehealthcheckdo)|
|**servicePortList**  <br>*optional*|< [ServicePortDO](#serviceportdo) > array|
|**serviceVolumeList**  <br>*optional*|< [ServiceVolumeDO](#servicevolumedo) > array|
|**startCommand**  <br>*optional*|string|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**taskStatus**  <br>*optional*|enum (STARTING, STOPING, DELETING, REDEPOLYING, UNDER_SCALE_UP, APPLICATION_DEPLOYING, APPLICATION_DELETING, APPLICATION_STARTING, APPLICATION_STOPPING, APPLICATION_REDEPLOYING, SERVICE_DELETING, SERVICE_STARTING, SERVICE_STOPPING, SERVICE_REDEPLOYING, SERVICE_ROLLING_UPGRADING, SERVICE_GRAY_UPGRADING, SERVICE_EXTENDING_HORIZONTAL, SERVICE_EXTENDING_VERTICAL, SERVICE_EXTENDING_ELASTIC, SERVICE_GRAY_UPGRADING_FINISH, SERVICE_GRAY_UPGRADING_CANCEL)|
|**tenantOid**  <br>*optional*|string|
|**upgradeFlag**  <br>*optional*|enum (NEW, OLD, IS_UPGRADE, IS_NOT_UPGRADE)|
|**useHostTimeZone**  <br>*optional*|boolean|
|**version**  <br>*optional*|integer(int32)|


<a name="servicemountconfigdto"></a>
### ServiceMountConfigDTO

|Name|Schema|
|---|---|
|**configGroup**  <br>*optional*|[ConfigGroupDTO](#configgroupdto)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**mountConfigList**  <br>*optional*|< [MountConfigDTO](#mountconfigdto) > array|
|**oid**  <br>*optional*|integer(int64)|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="serviceportdo"></a>
### ServicePortDO

|Name|Schema|
|---|---|
|**accessEntry**  <br>*optional*|[AccessEntryDO](#accessentrydo)|
|**accessOid**  <br>*optional*|integer(int64)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**forwardingRule**  <br>*optional*|string|
|**innerPort**  <br>*optional*|integer(int64)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**outerPort**  <br>*optional*|integer(int64)|
|**protocol**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="serviceportdto"></a>
### ServicePortDTO

|Name|Schema|
|---|---|
|**accessEntry**  <br>*optional*|[AccessEntryDTO](#accessentrydto)|
|**accessOid**  <br>*optional*|integer(int64)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**forwardingRule**  <br>*optional*|string|
|**innerPort**  <br>*optional*|integer(int64)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**outerPort**  <br>*optional*|integer(int64)|
|**protocol**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="servicescaleoutactiondto"></a>
### ServiceScaleOutActionDTO

|Name|Schema|
|---|---|
|**desired**  <br>*optional*|integer(int32)|
|**id**  <br>*optional*|integer(int64)|


<a name="servicescaleupdto"></a>
### ServiceScaleUpDTO

|Name|Schema|
|---|---|
|**cpuQuota**  <br>*optional*|integer(int32)|
|**memoryQuota**  <br>*optional*|integer(int32)|


<a name="servicesecuritypolicydo"></a>
### ServiceSecurityPolicyDO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**rule**  <br>*optional*|enum (ACCESS_IP_RANGE, APPLICATION, ACCESS_PORT)|
|**ruleValue**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|


<a name="serviceusagedto"></a>
### ServiceUsageDTO

|Name|Schema|
|---|---|
|**appId**  <br>*optional*|integer(int64)|
|**appName**  <br>*optional*|string|
|**cpuQuota**  <br>*optional*|integer(int32)|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**memoryQuota**  <br>*optional*|integer(int32)|
|**name**  <br>*optional*|string|
|**namespace**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**podTotal**  <br>*optional*|integer(int32)|
|**status**  <br>*optional*|enum (STARTING, RUNNING, STOP, ERROR, DELETING, DELETED, RESTARTING, REBUILDING, SERVICE_GRAY_UPGRADEING, SERVICE_GRAY_FINISH, SERVICE_GRAY_CANCEL, BLUE_GREEN_UPGRADING, BLUE_GREEN_FINISH, BLUE_GREEN_CANCEL)|
|**tenantId**  <br>*optional*|string|


<a name="servicevolumedo"></a>
### ServiceVolumeDO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**path**  <br>*optional*|string|
|**pvcName**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|
|**volumeId**  <br>*optional*|integer(int64)|


<a name="servicevolumedto"></a>
### ServiceVolumeDTO

|Name|Schema|
|---|---|
|**createTime**  <br>*optional*|string(date-time)|
|**createUser**  <br>*optional*|string|
|**deleted**  <br>*optional*|integer(int32)|
|**lastModifyTime**  <br>*optional*|string(date-time)|
|**lastModifyUser**  <br>*optional*|string|
|**name**  <br>*optional*|string|
|**oid**  <br>*optional*|integer(int64)|
|**path**  <br>*optional*|string|
|**pvcName**  <br>*optional*|string|
|**serviceId**  <br>*optional*|integer(int64)|
|**volumeId**  <br>*optional*|integer(int64)|


<a name="sseemitter"></a>
### SseEmitter

|Name|Schema|
|---|---|
|**timeout**  <br>*optional*|integer(int64)|



