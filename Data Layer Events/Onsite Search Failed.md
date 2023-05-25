# Onsite Search Failed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "view_search_results",
  "detailed_event": "Onsite Search Failed",
    "event_data": {
        "corrected_term": "<corrected_term>",
        "refine_catalog": "<refine_catalog>",
        "refine_geography": "<refine_geography>",
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
|event_data.search_term|string|Captures the search text used in on-site searches.|bluth, blue, red lobster|||||||




