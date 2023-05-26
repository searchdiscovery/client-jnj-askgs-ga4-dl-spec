# Form Viewed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_view",
  "detailed_event": "Form Viewed",
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

<p>This event should be dispatched whenever a form is in view on a users screen.</p>
<p><span class="hljs-string">"type"</span>: &nbsp;This parameter should be filled with which type of form is being filled out i.e. (Live chat, or submit a ticket)</p>
