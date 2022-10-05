# DocManager+ Documentation

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