# Page Rating

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "page_rating",
  "detailed_event": "Page Rating",
    "event_data": {
        "rating": "<rating>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.rating|string|Designates the rating of the page|positive, negative|||||||

## Attached Notes

<p>Fire when a user rates on article page via the thumbs up/thumbs down rating system&nbsp;</p>
<p>&nbsp;</p>
<p>"rating": 'positive'/'negative' (thumbs up = positive, thumbs down = negative)</p>
