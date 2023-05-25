# Download Link Clicked

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "file_download",
  "detailed_event": "Download Link Clicked",
    "event_data": {
        "component_ancestry": "<component_ancestry>",
        "file_extension": "<file_extension>",
        "file_name": "<file_name>",
        "identifier": "<identifier>",
        "link_url": "<link_url>",
        "region_ancestry": "<region_ancestry>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.component_ancestry|string|Captures the name or ID of the container within which download links are used.|Best Friends - Best Jeans, Puppy Love, Sail Away, Mens, Kids, Kids : Tops|||||||
|event_data.file_extension|string|Captures the type of file that was downloaded \(i.e. PDF, EPUB, DMG\).|pdf, doc, csv, dmp, zip|||||||
|event_data.file_name|string|Captures the file name associated with file downloads.|Year End 2012.pdf, Operating Instructions.doc`|||||||
|event_data.identifier|string|Captures the ID associated with download links used.|act now, cancel, ok, 3456, 8765|||||||
|event_data.link_url|string|The href URL of the link I clicked on|https:\/\/jnjgs.force.com\/s\/article-display?language=en\_US&name=Bank-name-branch-code-combinations&|||||||
|event_data.region_ancestry|string|Captures the name or ID of the region within which download links are used.|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||




