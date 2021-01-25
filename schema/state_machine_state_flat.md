
# state_machine_state_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|technicalName|string|true|none|none|
|name|string|true|none|none|
|stateMachineId|string(uuid)|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|stateMachine|[state_machine_flat](/schema/state_machine_flat)|false|none|Added since version: 6.0.0.0|
