# Example Data Templates


<details><summary>Type</summary>
<p>

###### Properties

| Property | Type |Description |
| --- | --- | --- |
| Type Of Model | "Cavalry" \| "Infantry" \| "Monster" | The types for this model.  |

###### Examples

```JSON5
"type": {
        "Type Of Model": {}
}
```

```JSON5
"type": {
        "Monster": {},
        "Infantry": {}
        ... // additonal types

}
```
</p>
</details>


<details><summary>Wargear</summary>
<p>

###### Properties

| Property | Type | Description |
| --- | --- | --- |
| Wargear Name | string | The name of the wargear in Capital Case format. |
| optional | boolean | Should this wargear be selectable by the user (true), or is it part of default wargear for the model (false). |
| points | number | The cost in points of the wargear. 0 if wargear is part of default wargear for the model |
| type | "Active" \| "Passive" | Is this wargear passive or active in its use. |
| userSelected | boolean | Default (false), changes when a user selects it (true).  |

###### Examples

```JSON5
"wargear": {
        // Selectable Wargear
        "Wargear Name": {
            "optional": true,
            "points": 5, 
            "style": "danger",
            "type": "Active",
            "userSelected": false
        },
        // Default Wargear
        "Wargear Name": {
            "optional": false,
            "points": 5, 
            "style": "neutral",
            "type": "Default",
            "userSelected": false
        }
}
```

```JSON5
"wargear": {
        "Crown Of Morgul": {
            "optional": true,
            "points": 25,
            "style": "warning",
            "type": "Passive",
            "userSelected": false
        },
        ... // additonal wargear
}
```
</p>
</details>



