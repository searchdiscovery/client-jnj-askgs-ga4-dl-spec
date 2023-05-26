# Form Submission Succeeded

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_complete",
  "detailed_event": "Form Submission Succeeded",
    "event_data": {
        "case_number": "<case_number>",
        "case_status": "<case_status>",
        "form_category": "<form_category>",
        "form_department": "<form_department>",
        "form_language": "<form_language>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.case_number|string|Case number associated with the live chat||||||||
|event_data.case_status|string|Case status associated with the live chat||||||||
|event_data.form_category|string|Form category associated with a submitted ticket||||||||
|event_data.form_department|string|Form department associated with the submitted ticket||||||||
|event_data.form_language|string|Language associated with a submitted ticket or live chat||||||||
|event_data.type|string|Captures the type of form \(i.e. demo, free trial, contact us\).|Address, Contact, Comment, Review, Payment|||||||

## Attached Notes

<p>This event should be dispatched whenever a user successfully submits their form.</p>
<p>&nbsp;</p>
<p><span class="hljs-string">"case_number"</span>: The case number associated with the case the user is inquiring about via live chat (if capturing this is possible)</p>
<p><span class="hljs-string">"case_status"</span>: The status of the case a user is inquiring about via live chat (if capturing this is possible)</p>
<p><span class="hljs-string">"form_category"</span>: Category associated with the form submission</p>
<p><span class="hljs-string">"form_department"</span>: Department associated with the form submission</p>
<p><span class="hljs-string">"form_language"</span>: Language selected in the form</p>
<p><span class="hljs-string">"type"</span>: This parameter should be filled with which type of form is being filled out i.e. (Live chat, or submit a ticket)</p>
