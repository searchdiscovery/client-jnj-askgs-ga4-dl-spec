# Select Search Result

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "select_search_result",
  "detailed_event": "Select Search Result",
    "event_data": {
        "corrected_term": "<corrected_term>",
        "refine_catalog": "<refine_catalog>",
        "refine_geography": "<refine_geography>",
        "results_count": "<results_count>",
        "search_slot": "<search_slot>",
        "search_term": "<search_term>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.corrected_term|string|Captures the search text used in on-site searches and what the search text was auto-corrected to.|bluth:blu, blue:blu, red lobster:rd lbstr|||||||
|event_data.refine_catalog|string|The value associated with the refine catalog search filter|i.e. Invoice Management & Reconciliation|||||||
|event_data.refine_geography|string|The value associated with the refine category search filter|i.e. United States|||||||
|event_data.results_count|string|Tracks the total number of results that are returned from an onsite search|i.e. 20|||||||
|event_data.search_slot|string|The position that the search result clicked is in relative to the total number of results returned for the search|i.e. 2|||||||
|event_data.search_term|string|Captures the search text used in on-site searches.|bluth, blue, red lobster|||||||

## Attached Notes

<p>Fire this event when a user clicks on a result from an onsite search</p>
<p>&nbsp;</p>
<p><span class="hljs-string">"corrected_term"</span>: The corrected search term if a user mispells their intended search or chooses an suggested search</p>
<p><span class="hljs-string">"refine_catalog"</span>: This will be populated with the value of the chosen catalog refinement after a search (HR, Payroll etc)</p>
<p><span class="hljs-string">"refine_geography"</span>: This will be populated with the value of the chosen catalog refinement after a search&nbsp;</p>
<p>"results_count": The total number of results that an onsite search yeilds&nbsp;</p>
<p><span class="hljs-string">"search_term"</span>: The term a user uses to search</p>
<p><span class="hljs-string">"search_slot"</span>: <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;The position that the search result clicked is in relative to the total number of results returned for the search&quot;}" data-sheets-userformat="{&quot;2&quot;:12865,&quot;3&quot;:{&quot;1&quot;:0},&quot;9&quot;:0,&quot;12&quot;:0,&quot;15&quot;:&quot;Arial&quot;,&quot;16&quot;:12}">The position that the search result clicked is in relative to the total number of results returned for the search</span></p>
<p>&nbsp;</p>
