# Form Submission Failed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_error",
  "detailed_event": "Form Submission Failed",
    "event_data": {
        "error_message": "<error_message>",
        "form_category": "<form_category>",
        "form_department": "<form_department>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.error_message|string|Captures the form error code or message associated with form errors.|Credit card declined, Required entries missing, EC3456, EC8976|||||||
|event_data.form_category|string|Form category associated with a submitted ticket||||||||
|event_data.form_department|string|Form department associated with the submitted ticket||||||||
|event_data.type|string|Captures the type of form \(i.e. demo, free trial, contact us\).|Address, Contact, Comment, Review, Payment|||||||

## Attached Notes

<p>This event should fire whenever a successful form submission is not achieved causing a fail for any reason.<br /><br /><span class="hljs-string">"error_message"</span>: This designates the reason for the fail i.e. (Blank field, email error, invalid entry)</p>
<p><span class="hljs-string">"form_category"</span>: Form category associated with a submitted ticket</p>
<p><span class="hljs-string">"form_department"</span>: Form department associated with the submitted ticket</p>
<p><span class="hljs-string">"type"</span>: This parameter should be filled with which type of form is being filled out i.e. (Live chat, or submit a ticket)</p>
