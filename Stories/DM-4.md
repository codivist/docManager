# DM-4

## Api End Point for Versioning a File

#### Description
In order for DocManager+ to track different versions of files, a new API endpoint will need to be implemented into our system. This will not be a exposed to 

#### Value
Users don't know it yet, but they will want to be able to see different versions of their documents in case they want to re-edit a part of it.

#### Acceptance Criteria
An empty call will be passed via POST to `/v1/files/{{file_id}}/version`

It will be acceptible to run this via an event from an API action as well.

On Success the following message should be returned:
```json
{
    "status": 201,
    "message": "Success",
}
```
On Error the following message should be returned:
```json
{
    "status": 400,
    "message": "Error",
    "error": {

    }
}
```

#### Notes
If using events to version the file, success and error messages should still be passed and logged.