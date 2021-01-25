
# dead_message_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|originalMessageClass|string|true|read-only|none|
|handlerClass|string|true|read-only|none|
|encrypted|boolean|true|read-only|none|
|errorCount|integer(int64)|true|read-only|none|
|nextExecutionTime|string(date-time)|true|read-only|none|
|exception|string|true|read-only|none|
|exceptionMessage|string|true|read-only|none|
|exceptionFile|string|true|read-only|none|
|exceptionLine|integer(int64)|true|read-only|none|
|scheduledTaskId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|scheduledTask|[scheduled_task_flat](/schema/scheduled_task_flat.md)|false|none|Added since version: 6.0.0.0|
