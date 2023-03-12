# Example Data Templates

<details><summary>Wargear</summary>
<p>

###### Properties
| Property | Type |Description |
| --- | --- | --- |
| optional | boolean | Should this wargear be selectable by the user (true), or is it part of default wargear for the model (false). |
| points | number | The cost in points of the wargear. 0 if wargear is part of default wargear for the model |
| type | "Active" \| "Passive" | Is this wargear passive or active in its use. |
| userSelected | boolean | Default (false), changes when a user selects it (true).  |

###### Examples
```JSON5
"wargear": {
        "Selectable Wargear": {
            "optional": true,
            "points": 5, 
            "style": "danger",
            "type": "Active",
            "userSelected": false
        },
        "Default Wargear": {
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



