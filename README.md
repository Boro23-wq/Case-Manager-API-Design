
# Case Manager API Documentation

The API retrieves information about case managers and their cases.

Contact Support:
 Name: Sintu Boro
 Email: sb394@njit.edu

<!--- If we have only one group/collection, then no need for the "ungrouped" heading -->


## Variables

| Key | Value | Type |
| --- | ------|-------------|
| baseUrl | http://localhost:3000 | string |



## Endpoints

* [case Managers](#case-managers)
    1. [Create a case manager.](#1-create-a-case-manager)
        * [Successfully created case manager.](#i-example-request-successfully-created-case-manager)
        * [Bad request. Required fields are missing.](#ii-example-request-bad-request-required-fields-are-missing)
        * [Not found.](#iii-example-request-not-found)
        * [Internal Server Error. Please try again later](#iv-example-request-internal-server-error-please-try-again-later)
    1. [Find all case managers.](#2-find-all-case-managers)
        * [Successfully retrieved all the case managers.](#i-example-request-successfully-retrieved-all-the-case-managers)
        * [Bad request.](#ii-example-request-bad-request)
        * [Not found.](#iii-example-request-not-found-1)
        * [Internal Server Error. Please try again later.](#iv-example-request-internal-server-error-please-try-again-later-1)
* [case Manager/{id}](#case-managerid)
    1. [Find case manager by ID.](#1-find-case-manager-by-id)
        * [Successfully retrieved case manager.](#i-example-request-successfully-retrieved-case-manager)
        * [Sorry! Couldn't find case manager with the ID provided.](#ii-example-request-sorry-couldnt-find-case-manager-with-the-id-provided)
        * [Sorry! Case manager with the ID not found.](#iii-example-request-sorry-case-manager-with-the-id-not-found)
        * [Internal server error. Please try again later.](#iv-example-request-internal-server-error-please-try-again-later-2)
    1. [Update a case manager.](#2-update-a-case-manager)
        * [Successfully updated case manager with the provided ID.](#i-example-request-successfully-updated-case-manager-with-the-provided-id)
        * [Sorry! Couldn't find case manager with the ID provided.](#ii-example-request-sorry-couldnt-find-case-manager-with-the-id-provided-1)
        * [Sorry! Case manager with the ID not found.](#iii-example-request-sorry-case-manager-with-the-id-not-found-1)
        * [Internal server error. Please try again later.](#iv-example-request-internal-server-error-please-try-again-later-3)
    1. [Delete a case manager.](#3-delete-a-case-manager)
        * [Case manager deleted sucessfully.](#i-example-request-case-manager-deleted-sucessfully)
        * [Sorry! Couldn't find case manager with the ID provided.](#ii-example-request-sorry-couldnt-find-case-manager-with-the-id-provided-2)
        * [Sorry! Case manager with the ID not found.](#iii-example-request-sorry-case-manager-with-the-id-not-found-2)
        * [Internal server error. Please try again later.](#iv-example-request-internal-server-error-please-try-again-later-4)

--------



## case Managers



### 1. Create a case manager.


Creates a new case manager using the input provided and add it to the system.


***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{baseUrl}}/caseManagers
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| Accept | application/json |  |



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "consectetur Duis sit",
      "category": "amet eu adipisicing in",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "pariatur ut est id",
      "category": "irure consequat Duis commodo",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***More example Requests/Responses:***


#### I. Example Request: Successfully created case manager.



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



#### I. Example Response: Successfully created case manager.
```js
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```


***Status Code:*** 201

<br>



#### II. Example Request: Bad request. Required fields are missing.



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 400

<br>



#### III. Example Request: Not found.



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 404

<br>



#### IV. Example Request: Internal Server Error. Please try again later



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 500

<br>



### 2. Find all case managers.


Get all the case managers and their cases recorded in the system.


***Endpoint:***

```bash
Method: GET
Type: 
URL: {{baseUrl}}/caseManagers
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 99033173 |  |
| perPage | 99033173 |  |



***More example Requests/Responses:***


#### I. Example Request: Successfully retrieved all the case managers.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 99033173 |  |
| perPage | 99033173 |  |



***Body: None***



#### I. Example Response: Successfully retrieved all the case managers.
```js
[
  {
    "username": "johndoe",
    "firstName": "John",
    "lastName": "Doe",
    "email": "johndoe@cm.io",
    "phone": 8623817665,
    "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
    "createdAt": "2021-01-30T08:30:00Z",
    "modifiedAt": "2021-01-31T08:30:00Z",
    "cases": [
      {
        "status": "adipisicing conseq",
        "category": "nulla nostrud",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {},
        "solution": {},
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          }
        ]
      },
      {
        "status": "velit Duis",
        "category": "occaecat id",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {},
        "solution": {},
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          }
        ]
      }
    ]
  },
  {
    "username": "johndoe",
    "firstName": "John",
    "lastName": "Doe",
    "email": "johndoe@cm.io",
    "phone": 8623817665,
    "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
    "createdAt": "2021-01-30T08:30:00Z",
    "modifiedAt": "2021-01-31T08:30:00Z",
    "cases": [
      {
        "status": "sunt culpa",
        "category": "cillum consequat",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {},
        "solution": {},
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          }
        ]
      },
      {
        "status": "labore ea tempor ipsum",
        "category": "sint id minim",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {},
        "solution": {},
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          }
        ]
      }
    ]
  }
]
```


***Status Code:*** 200

<br>



#### II. Example Request: Bad request.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 99033173 |  |
| perPage | 99033173 |  |



***Body: None***



***Status Code:*** 400

<br>



#### III. Example Request: Not found.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 99033173 |  |
| perPage | 99033173 |  |



***Body: None***



***Status Code:*** 404

<br>



#### IV. Example Request: Internal Server Error. Please try again later.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 99033173 |  |
| perPage | 99033173 |  |



***Body: None***



***Status Code:*** 500

<br>



## case Manager/{id}



### 1. Find case manager by ID.


Returns a single case manager with the provided ID.


***Endpoint:***

```bash
Method: GET
Type: 
URL: {{baseUrl}}/caseManager/:id
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of case manager to return. |



***More example Requests/Responses:***


#### I. Example Request: Successfully retrieved case manager.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of case manager to return. |



***Body: None***



#### I. Example Response: Successfully retrieved case manager.
```js
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```


***Status Code:*** 200

<br>



#### II. Example Request: Sorry! Couldn't find case manager with the ID provided.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of case manager to return. |



***Body: None***



***Status Code:*** 400

<br>



#### III. Example Request: Sorry! Case manager with the ID not found.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of case manager to return. |



***Body: None***



***Status Code:*** 404

<br>



#### IV. Example Request: Internal server error. Please try again later.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of case manager to return. |



***Body: None***



***Status Code:*** 500

<br>



### 2. Update a case manager.


Update details of a case manager using ID.


***Endpoint:***

```bash
Method: PUT
Type: RAW
URL: {{baseUrl}}/caseManager/:id
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| Accept | application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be updated. |



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***More example Requests/Responses:***


#### I. Example Request: Successfully updated case manager with the provided ID.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be updated. |



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



#### I. Example Response: Successfully updated case manager with the provided ID.
```js
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```


***Status Code:*** 201

<br>



#### II. Example Request: Sorry! Couldn't find case manager with the ID provided.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be updated. |



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 400

<br>



#### III. Example Request: Sorry! Case manager with the ID not found.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be updated. |



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 404

<br>



#### IV. Example Request: Internal server error. Please try again later.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be updated. |



***Body:***

```js        
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "caseManagerId": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "status": "dolore officia in tempor laboris",
      "category": "incididunt fugiat ipsum do",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "est",
      "category": "Duis in nulla qui cillum",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {},
      "solution": {},
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "mileStoneId": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "activityId": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 500

<br>



### 3. Delete a case manager.


Delete an existing case manager.


***Endpoint:***

```bash
Method: DELETE
Type: 
URL: {{baseUrl}}/caseManager/:id
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be deleted. |



***More example Requests/Responses:***


#### I. Example Request: Case manager deleted sucessfully.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be deleted. |



***Body: None***



#### I. Example Response: Case manager deleted sucessfully.
```js
"290cdddc-31af-481c-9000-2ab4eabeebaf"
```


***Status Code:*** 204

<br>



#### II. Example Request: Sorry! Couldn't find case manager with the ID provided.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be deleted. |



***Body: None***



***Status Code:*** 400

<br>



#### III. Example Request: Sorry! Case manager with the ID not found.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be deleted. |



***Body: None***



***Status Code:*** 404

<br>



#### IV. Example Request: Internal server error. Please try again later.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| id | -78323989 | (Required) ID of the case manager to be deleted. |



***Body: None***



***Status Code:*** 500

<br>



---
[Back to top](#case-manager-api-documentation)

>Generated at 2022-10-20 22:12:05 by [docgen](https://github.com/thedevsaddam/docgen)
