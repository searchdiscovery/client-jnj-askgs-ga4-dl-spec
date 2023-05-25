# CTA Link Clicked

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "click",
  "detailed_event": "CTA Link Clicked",
    "event_data": {
        "component_ancestry": "<component_ancestry>",
        "identifier": "<identifier>",
        "link_url": "<link_url>",
        "outbound": <outbound>,
        "region_ancestry": "<region_ancestry>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.component_ancestry|string|Captures the name or ID of the container within which CTA links are used.|Best Friends - Best Jeans, Puppy Love, Sail Away, Mens, Kids, Kids : Tops|||||||
|event_data.identifier|string|Captures the ID associated with CTA links used.|act now, cancel, ok, 3456, 8765|||||||
|event_data.link_url|string|The href URL of the link I clicked on|https:\/\/jnjgs.force.com\/s\/article-display?language=en\_US&name=Bank-name-branch-code-combinations&|||||||
|event_data.outbound|boolean|is the CTA click an outbound click||||||||
|event_data.region_ancestry|string|Captures the name or ID of the region within which CTA links are used.|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||




