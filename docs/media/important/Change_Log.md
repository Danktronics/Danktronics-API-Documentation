# Change Log

## Removal of uniform data structure and ISO creation times

### TBD

The data structure that was returned by all API endpoints will no longer be present in favor of only returning the data. This was a bloated feature of the API. Also all objects returned by the API will no longer contain ISO-8601 `created_at` fields in favor of parsing the snowflake ID for a instantaneous timestamp.