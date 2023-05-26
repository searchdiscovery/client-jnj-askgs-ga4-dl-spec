# Form Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_start",
  "detailed_event": "Form Started",
    "event_data": {
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.type|string|Captures the type of form \(i.e. demo, free trial, contact us\).|Address, Contact, Comment, Review, Payment|||||||

## Attached Notes

<p>This event should fire whenever a user starts to fill out a form on the site. This should only fire once/form.<br /><br />"type": This parameter should be filled with which type of form is being filled out i.e. (Live chat, or submit a ticket)</p>
