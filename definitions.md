
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



