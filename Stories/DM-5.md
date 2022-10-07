# DM-5

## Database Migration via Lumen/Laravel

### Magnitude 5

#### Description
Database changes will need to be made for the DocManager+ feature. Our DevOps team requires that the migration changes be fully tested, and run on a test server before running in production. 

#### Value
Database migrations are key for the DocManager+ feature to be successful. This is behind the scenes and users will not know it's even there.

#### Acceptance Criteria
DB migrations will be created in the Laravel format
```
php artisan make:migration create_files_table
```
etc. for each additional table listed in the [Table Model diagram](../tables.md)


Each migration MUST be able to fully roll back to the previous state before it was run.
Each Database change must be accompanied by a migration with the following title format of:
* YYYY_MM_DD_100000_create_files_table.php 

#### Notes
