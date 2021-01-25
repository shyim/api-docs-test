
# state_machine_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|technicalName|string|true|none|none|
|name|string|true|none|none|
|customFields|object|false|none|none|
|initialStateId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|states|[state_machine_state_flat](/schema/state_machine_state_flat.md)|false|none|Added since version: 6.0.0.0|
|transitions|[state_machine_transition_flat](/schema/state_machine_transition_flat.md)|false|none|Added since version: 6.0.0.0|
|historyEntries|[state_machine_history_flat](/schema/state_machine_history_flat.md)|false|none|Added since version: 6.0.0.0|
