# DM-7

## S3 Bucket Creation

### Magnitude 3

#### Description
As per RimSys standards, all documents must be stored in S3 buckets named for each customer. These buckets must be set up dynamically if the user is uploading their first file.

#### Value
Offsite data storage will save us money and the user time when uploading and downloading files. This also keeps us from being liable.

#### Acceptance Criteria
* S3 bucket must be created upon initialization of the user's first file upload or before
* S3 bucket naming convention must follow our existing standards
* Empty buckets are fine for now

#### Notes



[Back to Overview](../readme.md)