
# state_machine_history_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|stateMachineId|string(uuid)|true|none|none|
|entityName|string|true|none|none|
|entityId|object|true|none|none|
|fromStateId|string(uuid)|true|none|none|
|toStateId|string(uuid)|true|none|none|
|transitionActionName|string|false|none|none|
|userId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|stateMachine|[state_machine_flat](/schema/state_machine_flat.md)|false|none|Added since version: 6.0.0.0|
|fromStateMachineState|[state_machine_state_flat](/schema/state_machine_state_flat.md)|false|none|Added since version: 6.0.0.0|
|toStateMachineState|[state_machine_state_flat](/schema/state_machine_state_flat.md)|false|none|Added since version: 6.0.0.0|
