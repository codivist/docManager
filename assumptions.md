### DocManager+ Assumtions & Dependancies

#### Tech Assumtions
In order to facilitate an immediate start on this project we will be assuming the following items:
1. We will use existing tech & infrastructure
    1. PHP/Laravel, Nuxt/Vue, MySQL, and AWS/S3
    1. Will keep costs down
1. Database infrastructure will be altered minimally
    1. Result should have minimal to no downtime
1. Will need to create a new S3 bucket for documents
1. Will need to add new permissions/gates in API
    1. As well as checks in the front end
1. Current CI/CD procedures allow us to integrate this project seemlessly
1. Unit tests must be used to make sure points of the system are not breaking when coding or re-factoring


#### Dependancies
* Database migrations will need to be built in with proper roll-backs in place
* Vue Components for file manipulation will need to be updated
* The backend team will need 2 full sprints without interuption
    * Depending on interuptions, could push API changes causing delay in MVP
    * The front end development could be affected by this delay as well
* The Product team has promised cake and ice cream if project is done early
* Daniel B. is wrapping up some ADA compliant work on the UDI project and isn't available until Sprint 2 at the earliest
* QA will test as project develops


