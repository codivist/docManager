# DM-3

## Api End Point for Downloading a File

#### Description
In order for DocManager+ to download files, a new API endpoint will need to be implemented into our system.

#### Value
Users will want to be able to download their files for personal reasons. Just in case they want to print it.

#### Acceptance Criteria
A call will be passed via GET to `/v1/files/{{file_id}}/download`

On Success the following message should be returned:
```json
{
    "status": 200,
    "message": "Your file will begin downloading shortly.",
}
```
On Error the following message should be returned:
```json
{
    "status": 404,
    "message": "There file could not be found."
}
```

#### Notes