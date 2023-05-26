# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_load_started",
  "detailed_event": "Page Load Started",
    "page_data": {
        "country": "<country>",
        "language": "<language>",
        "name": "<name>",
        "page_location": "<page_location>",
        "page_path": "<page_path>",
        "page_referrer": "<page_referrer>",
        "page_title": "<page_title>",
        "site_section": "<site_section>",
        "type": "<type>"
    },
    "user_data": {
        "user_email": "<user_email>",
        "user_id": "<user_id>",
        "user_leader": <user_leader>,
        "user_level": "<user_level>",
        "user_paygrade": "<user_paygrade>",
        "user_region": "<user_region>",
        "user_sector": "<user_sector>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.country|string|The country associated with the current page.|US, CA, FR, UK|||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.|en-us, en-gb, ch-cn, fr-ca, fr-fr|||||||
|page_data.name|string|Captures the name of the page the user is on|product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page_data.page_location|string|The URL of the page currently being viewed. This value will include the full, unaltered URL of the page\/screen the user is currently viewing, including query parameters, fragments, etc., for example https:\/\/www.example.com\/home?user=true&audience=test\#aboutus.|https:\/\/www.example.com\/home?user=true&audience=test\#aboutus|||||||
|page_data.page_path|string|Captures the path portion of the page URL.||||||||
|page_data.page_referrer|string|DLV \| page\_referrer||||||||
|page_data.page_title|string|The title of the page currently being viewed, generally available in &lt;title&gt;.||||||||
|page_data.site_section|string|The section of the site that the current page resides in. site\_section2 through site\_section5can also be used if the site has many sections.||||||||
|page_data.type|string|The type of page currently viewed.|home, pdp, article|||||||
|user_data.user_email|string|Stores the email of the logged in user||||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated.|123456, abc123|||||||
|user_data.user_leader|boolean|Designates if the user is a leader in the organization||||||||
|user_data.user_level|string|Designates the level of the user||||||||
|user_data.user_paygrade|string|Designates the paygrade of the user||||||||
|user_data.user_region|string|Designates the region the user is in||||||||
|user_data.user_sector|string|Designates the sector the user is in||||||||

## Attached Notes

<p>This should be fired on every page BEFORE any other event</p>
<p>&nbsp;</p>
<p><span class="hljs-string">"language"</span>: Language that the page is being viewed in</p>
<p><span class="hljs-string">"page_location"</span>: Full URL of the page</p>
<p><span class="hljs-string">"page_path"</span>: Portion of the URL after the hostname</p>
<p><span class="hljs-string">"page_referrer"</span>: Full URL of the page viewed prior to the current page</p>
<p><span class="hljs-string">"page_title"</span>: Title of the page&nbsp;</p>
<p><span class="hljs-string">"site_section"</span>: Page category - either '<span style="font-weight: 400;">Home', 'My requests', 'Submit a request', 'Search', 'Article')</span></p>
<p>&nbsp;</p>
<p><span class="hljs-string">"user_email"</span>: Hashed user email address (to be used in the future for Qualtrics)</p>
<p><span class="hljs-string">"user_id"</span>: J&amp;J specific user id (wwid)</p>
<p><span class="hljs-string">"user_leader"</span>: Boolean - is this person in a management position?&nbsp;</p>
<p><span class="hljs-string">"user_level"</span>: J&amp;J specific position level</p>
<p><span class="hljs-string">"user_paygrade"</span>: J&amp;J specific paygrade grouping</p>
<p><span class="hljs-string">"user_region"</span>: J&amp;J specific region</p>
<p><span class="hljs-string">"user_sector"</span>: J&amp;J specific department specification</p>
