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
        "identifier": "<identifier>",
        "link_url": "<link_url>",
        "outbound": <outbound>,
        "region_ancestry": "<region_ancestry>",
        "subregion": "<subregion>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.identifier|string|Captures the ID associated with CTA links used.|act now, cancel, ok, 3456, 8765|||||||
|event_data.link_url|string|The href URL of the link I clicked on|https:\/\/jnjgs.force.com\/s\/article-display?language=en\_US&name=Bank-name-branch-code-combinations&|||||||
|event_data.outbound|boolean|is the CTA click an outbound click||||||||
|event_data.region_ancestry|string|Captures the name or ID of the region within which CTA links are used.|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||
|event_data.subregion|string|The region within the main region \(ex. navigation, main content, side panel\)|i.e. navigation, main content, side panel|||||||
|event_data.type|string|Captures the type of profile update \(i.e. change email\) completed by the user.|email, address, phone, subscriptions|||||||

## Attached Notes

<p><span style="font-weight: 400;">Fire when a user clicks on any of the following link elements:</span></p>
<ul>
<li><span style="font-weight: 400;">Navigation</span></li>
<li><span style="font-weight: 400;">Select a topic tiles</span></li>
<li><span style="font-weight: 400;">Language Selection</span></li>
<li><span style="font-weight: 400;">Location Selection</span></li>
<li><span style="font-weight: 400;">Tab Click (Open/Resolve/Closed on My Requests page)</span></li>
<li><span style="font-weight: 400;">Sort</span></li>
<li><span style="font-weight: 400;">Initial Contact Initiation (Submit a ticket, Live Chat, Contact by phone, Contact IT)</span></li>
<li><span style="font-weight: 400;">Outbound Resources</span></li>
</ul>
<p><span style="font-weight: 400;">These should also be the categories reflected in the click 'type' parameter.&nbsp;</span></p>
<p><span style="font-weight: 400;">Do not fire on a file download click, page rating, select search result or form submit click</span></p>
<p>&nbsp;</p>
<p>&nbsp;<span class="hljs-string">"identifier"</span>: Should reflect the exact link being clicked - link text will often satisfy this value</p>
<p><span class="hljs-string">"link_url"</span>: Href url of the link being clicked</p>
<p><span class="hljs-string">"outbound"</span>: Boolean</p>
<p><span class="hljs-string">"region_ancestry"</span>: Top level region of the page - either 'Header', 'Body', or 'Footer'</p>
<p><span class="hljs-string">"subregion"</span>: Secondary region of the top level region -&nbsp;<em><span style="font-weight: 400;">either 'Navigation', 'Main Content', 'Side panel'</span></em></p>
<p><span class="hljs-string">"type"</span>: See note above</p>
