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
        "file_extension": "<file_extension>",
        "file_name": "<file_name>",
        "identifier": "<identifier>",
        "link_url": "<link_url>",
        "region_ancestry": "<region_ancestry>",
        "subregion": "<subregion>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.file_extension|string|Captures the type of file that was downloaded \(i.e. PDF, EPUB, DMG\).|pdf, doc, csv, dmp, zip|||||||
|event_data.file_name|string|Captures the file name associated with file downloads.|Year End 2012.pdf, Operating Instructions.doc`|||||||
|event_data.identifier|string|Captures the ID associated with download links used.|act now, cancel, ok, 3456, 8765|||||||
|event_data.link_url|string|The href URL of the link I clicked on|https:\/\/jnjgs.force.com\/s\/article-display?language=en\_US&name=Bank-name-branch-code-combinations&|||||||
|event_data.region_ancestry|string|Captures the name or ID of the region within which download links are used.|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||
|event_data.subregion|string|The region within the main region \(ex. navigation, main content, side panel\)|i.e. navigation, main content, side panel|||||||

## Attached Notes

<p><span class="hljs-string">Fire this event whenever a user clicks on a download file link.</span></p>
<p>&nbsp;</p>
<p><span class="hljs-string">"file_extension"</span>: Designates the file type for example (.pdf, .csv) etc</p>
<p><span class="hljs-string">"file_name"</span>: This is the human readable name of the downloaded file&nbsp;</p>
<p><span class="hljs-string">"identifier"</span>: This should reflect the exact file that is being downloaded - often satisfied by the link text</p>
<p><span class="hljs-string">"link_url"</span>: The full href of the download link</p>
<p><span class="hljs-string">"region_ancestry"</span>: Top level region of the page - either 'Header', 'Body', or 'Footer'</p>
<p><span class="hljs-string">"subregion"</span>: Secondary region of the top level region -&nbsp;<em>either 'Navigation', 'Main Content', 'Side panel'</em></p>
