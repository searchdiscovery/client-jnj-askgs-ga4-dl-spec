# Onsite Search Succeeded

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "view_search_results",
  "detailed_event": "Onsite Search Succeeded",
    "event_data": {
        "corrected_term": "<corrected_term>",
        "refine_catalog": "<refine_catalog>",
        "refine_geography": "<refine_geography>",
        "results_count": "<results_count>",
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
|event_data.search_term|string|Captures the search text used in on-site searches.|bluth, blue, red lobster|||||||

## Attached Notes

<p>This event should be sent when at least one search result is succesfully sent back after an onsite search&nbsp;</p>
<p>&nbsp;</p>
<p><span class="hljs-string">"corrected_term"</span>: The corrected search term if a user mispells their intended search or chooses an suggested search</p>
<p><span class="hljs-string">"refine_catalog"</span>: This will be populated with the value of the chosen catalog refinement after a search (HR, Payroll etc)</p>
<p><span class="hljs-string">"refine_geography"</span>: This will be populated with the value of the chosen catalog refinement after a search&nbsp;</p>
<p>"results_count": The total number of results that an onsite search yeilds&nbsp;</p>
<p><span class="hljs-string">"search_term"</span>: The term a user uses to search</p>
<p>&nbsp;</p>
