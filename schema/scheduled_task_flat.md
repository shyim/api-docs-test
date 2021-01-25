
# scheduled_task_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|scheduledTaskClass|string|true|none|none|
|runInterval|integer(int64)|true|none|none|
|status|string|true|none|none|
|lastExecutionTime|string(date-time)|false|none|none|
|nextExecutionTime|string(date-time)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|deadMessages|[dead_message_flat](/schema/dead_message_flat.md)|false|none|Added since version: 6.0.0.0|
