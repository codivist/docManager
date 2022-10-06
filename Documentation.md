# DocManager+ Documentation
__*This is an example of documentation that "could" have been created from the beginning of the project planning*__

## 1. Goals of this Documentation
DocManager+ is a feature request that will allow users to:
1. Add/Upload documents
1. Version documents
1. Add tasks to a document
1. Download a document


### 1.1 Requirements Overview
The main purpose of DocManager+ is to allow users to upload a document to their account, make changes to the document and allow tasks to be added to the document, then download their own document when needed.

DocManager+ is used to Track, manage and download important documents for getting health care devices approved and to market in a relative quick manner.

#### Main features
* Upload and store documents
* Track versions of the document if changes are made to a document
* Add tasks to a document and track the status of tasks at the document level
* Download a document

The feature must authentication that is already in place for a user. As well as other security practices already in place.

Most users want to store more than one document. The feature should be able to keep track of storing 1 or more documents. 

Users will want to attach tasks to a document so they know if Sally in Accounting has approved their party on the 28th. Attaching 1 to 25 tasks to a document, and show the status if completed or not.

If a user edits a document, the feature can show how many times it has been revised and see what changes were made.

Users must be able to download their document at anytime and independant of any task status.

### 1.2 Qualitiy Goals
| Priorities    | Quality Goal  | Scenario |
|---------------|---------------|----------|
| 1             | Upload File   | Upload form properly places file on server and is named correctly and returns success or failure message |
| 1             | Add Task(s)   | Tasks should only be associated to the selected document |
| 2             | Download file | Link to download file should be visible. Downloads selected file when clicked. |
| 2             | Version Track file | Record and show revisions to document along with date. |

### 1.3 Stakeholders
| Role  | Goal, Intention |
|-------|-----------------|
| User  | Uses the feature to add files and track tasks so they can see what needs to be done to finish approval of devices | 
| Another User | More file tracking and downloading |

## 2. Constraints
DocManager+ shall be:
* Platform independant and run on any browser
* Easy to use
* Responsive and quick

### 2.1 Technical Constraints
| Constraint | Background/Motivation |
|------------|-----------------------|
| API backend implementation in Lumen | The backend of this feature must be developed in Lumen. The api interface should be language and framework agnostic.
| DB should use MySQL & Redis | For this feature to be usable on multiple devices it should utilize MySQL as the DB. Redis should be considered as session management to help speed up the front end.
| Front end implementation in Nuxt/Vue.js | The front end of this feature should be developed in Nuxt/Vue.js and consume the api backend, utilizing current company security standards. |
| AWS will be used as document storage | To keep files secure, quickly retreivable and organized. The feature should utilize AWS and S3 storage to store documents and retreive them. |
| CI/CD | Since the main product is already using github, this feature should use github actions to pipeline pushes from the `main` branch into production. |
| Unit Testing | Unit tests must be included in both backend and front end development

### 2.2 Organizational Constraints
| Constraint | Background/Motivation |
|------------|-----------------------|
| Teams         | Team A will be working on the backend, while Team B will be working on the front end. |
| Time Schedule | Team A is currently finishing up a feature for Brad. Team B is ready to start implementing the basic design |
| Design        | UI is currently in design |
| Testing       | Daniel has learned all about front end linting and testing so this should not slow the team down |
| Version Control & Code management | A private git repo will keep a complete history and track all code in this feature |


## 3. Context

## 4. Solution Strategy

## 5. 
## 6. 
## 7. 
## 8. 
## 9. 
## 10. 








