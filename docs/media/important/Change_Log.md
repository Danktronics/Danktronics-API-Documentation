# Change Log

## Limiting Data Retrieval

### TBD

* Now by default the Images and QuickLinks GET endpoint will return 10 items
* Images and QuickLinks GET endpoint can be customized with before, after, and limit (to retrieve more data)
* Images and QuickLinks GET endpoint return the total number of items owned by the current user (as this would be taxing to calculate with multiple requests)

## Removal of uniform data structure and ISO creation times

### 5/21/2020

* The data structure that was returned by all API endpoints will no longer be present in favor of only returning the data.
* All objects returned by the API will no longer contain ISO-8601 `created_at` fields in favor of parsing the snowflake ID for an instantaneous timestamp.
* `quickURL` (in QuickLinks) has been renamed to `quick_url` to conform with the rest of the API.
* `url` (in QuickLinks) has been renamed to `redirect_url` for clarity.
* Fields that return IDs will now have a suffix of `_id` (for example: `owner_id` instead of `owner`).
