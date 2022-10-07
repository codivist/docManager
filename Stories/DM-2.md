# DM-2

## Api End Point for Adding Task to File

#### Description
In order for DocManager+ to attach tasks to a file, a new API endpoint will need to be implemented into our system.

#### Value
Adding the new api end points will result in keeping personal files away from public files. 

#### Acceptance Criteria
The following items must be passed via POST to `/v1/files/{{file_id}}/task`
```json
{
    "user_id": "21d796b7-f180-499c-8783-ea2221b21138",
    "task_name": "my task name",
    "is_completed": false,
}
```
On Success the following message should be returned:
```json
{
    "status": 201,
    "message": "Task has been added.",
    "data": {
        "file_path": "S3 bucket url/path/to/file",
        "file_name": "myFile.docx",
        "file_url": "https://full-s3-url/to/myFile.docx"
    }
}
```
On Error the following message should be returned:
```json
{
    "status": 422,
    "message": "There was a problem adding your task.",
    "error": {
        "task_name": "Task must not be empty"
    }
}
```

#### Notes