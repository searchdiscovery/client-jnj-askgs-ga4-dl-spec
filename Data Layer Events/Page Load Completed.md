# Page Load Completed

### Page Load Completed is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the last event pushed in the page load event sequence.

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "page_view",
  "detailed_event": "Page Load Completed"
});
```





## Attached Notes

<p>This event should be sent when the page is loaded. This should be send AFTER the page load started event.&nbsp;</p>
