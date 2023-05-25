# Scroll

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "scroll",
  "detailed_event": "Scroll",
    "event_data": {
        "scroll_milestone": "<scroll_milestone>",
        "scroll_type": "<scroll_type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.scroll_milestone|string|How far down the page\/window the user has scrolled|25, 50, 75, 100|||||||
|event_data.scroll_type|string|Identifies whether a user is scrolling on the page or the request window|Value should be either "Page" "My Requests"|||||||




