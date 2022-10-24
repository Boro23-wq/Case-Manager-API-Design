
# Case Manager API Collection

The API retrieves information about case managers and their cases.

Contact Support:
 - **Name:** Sintu Boro
 - **Email:** sb394@njit.edu

<!--- If we have only one group/collection, then no need for the "ungrouped" heading -->


## Variables

| Key | Value | Type |
| --- | ------|-------------|
| baseUrl | http://localhost:3000 | string |



## Endpoints

* [casemanagers](#casemanagers)
    1. [{id}](#1-id)
    1. [Create a case manager.](#2-create-a-case-manager)
        * [Successfully created case manager.](#i-example-request-successfully-created-case-manager)
        * [Bad request. Required fields are missing.](#ii-example-request-bad-request-required-fields-are-missing)
        * [Not found.](#iii-example-request-not-found)
        * [Internal Server Error. Please try again later](#iv-example-request-internal-server-error-please-try-again-later)
    1. [Find all case managers.](#3-find-all-case-managers)
        * [Successfully retrieved all the case managers.](#i-example-request-successfully-retrieved-all-the-case-managers)
        * [Bad request.](#ii-example-request-bad-request)
        * [Not found.](#iii-example-request-not-found-1)
        * [Internal Server Error. Please try again later.](#iv-example-request-internal-server-error-please-try-again-later-1)
* [cases](#cases)
    1. [{id}](#1-id-1)
    1. [Create a case.](#2-create-a-case)
        * [Successfully created case.](#i-example-request-successfully-created-case)
        * [Bad request. Required fields are missing.](#ii-example-request-bad-request-required-fields-are-missing-1)
        * [Not found.](#iii-example-request-not-found-2)
        * [Internal Server Error. Please try again later](#iv-example-request-internal-server-error-please-try-again-later-2)
    1. [Find all cases.](#3-find-all-cases)
        * [Successfully retrieved all the cases.](#i-example-request-successfully-retrieved-all-the-cases)
        * [Bad request.](#ii-example-request-bad-request-1)
        * [Not found.](#iii-example-request-not-found-3)
        * [Internal Server Error. Please try again later.](#iv-example-request-internal-server-error-please-try-again-later-3)

--------



## casemanagers



### 1. {id}



***Endpoint:***

```bash
Method: 
Type: 
URL: 
```



### 2. Create a case manager.


Create a new case manager using the input provided and add it to the system.


***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{baseUrl}}/casemanagers
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
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    },
    {
      "status": "Active",
      "category": "Eye",
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientDetail": {
        "firstName": "Matt",
        "lastName": "Turner",
        "userName": "mattturner10",
        "phone": 9452877662,
        "email": "mattturner@gmail.com",
        "id": "46005a82-a612-4dc1-9279-7215df6895cd"
      },
      "solution": {
        "solutionSubject": "Operate eye disease.",
        "investigation": "Diseases on the left eye and abnormal eye development and function.",
        "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
      },
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {
        "firstName": "Katherine",
        "lastName": "Marshall",
        "phone": 8452877665,
        "email": "kathmarshall@hm.io",
        "id": "26005a82-a612-4dc1-9279-7215df6895cd",
        "assignedOn": "2021-03-30T08:30:00Z",
        "profession": "Ophthalmologists"
      },
      "milestones": [
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        },
        {
          "description": "Home therapy for left eye before surgery.",
          "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
          "createdAt": "2022-10-21T01:12:23.926Z"
        }
      ],
      "activities": [
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        },
        {
          "description": "Uploaded X-Ray report.",
          "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
          "createdAt": "2022-10-21T01:14:27.516Z"
        }
      ]
    }
  ]
}
```



***Status Code:*** 500

<br>



### 3. Find all case managers.


Get all the case managers and their cases recorded in the system.


***Endpoint:***

```bash
Method: GET
Type: 
URL: {{baseUrl}}/casemanagers
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 | Page number to paginate. |
| perPage | 10 | Total items to retrive at once. |



***More example Requests/Responses:***


#### I. Example Request: Successfully retrieved all the case managers.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 |  |
| perPage | 10 |  |



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
        "status": "Active",
        "category": "Eye",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {
          "firstName": "Matt",
          "lastName": "Turner",
          "userName": "mattturner10",
          "phone": 9452877662,
          "email": "mattturner@gmail.com",
          "id": "46005a82-a612-4dc1-9279-7215df6895cd"
        },
        "solution": {
          "solutionSubject": "Operate eye disease.",
          "investigation": "Diseases on the left eye and abnormal eye development and function.",
          "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
        },
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {
          "firstName": "Katherine",
          "lastName": "Marshall",
          "phone": 8452877665,
          "email": "kathmarshall@hm.io",
          "id": "26005a82-a612-4dc1-9279-7215df6895cd",
          "assignedOn": "2021-03-30T08:30:00Z",
          "profession": "Ophthalmologists"
        },
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          }
        ]
      },
      {
        "status": "Active",
        "category": "Eye",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {
          "firstName": "Matt",
          "lastName": "Turner",
          "userName": "mattturner10",
          "phone": 9452877662,
          "email": "mattturner@gmail.com",
          "id": "46005a82-a612-4dc1-9279-7215df6895cd"
        },
        "solution": {
          "solutionSubject": "Operate eye disease.",
          "investigation": "Diseases on the left eye and abnormal eye development and function.",
          "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
        },
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {
          "firstName": "Katherine",
          "lastName": "Marshall",
          "phone": 8452877665,
          "email": "kathmarshall@hm.io",
          "id": "26005a82-a612-4dc1-9279-7215df6895cd",
          "assignedOn": "2021-03-30T08:30:00Z",
          "profession": "Ophthalmologists"
        },
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
        "status": "Active",
        "category": "Eye",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {
          "firstName": "Matt",
          "lastName": "Turner",
          "userName": "mattturner10",
          "phone": 9452877662,
          "email": "mattturner@gmail.com",
          "id": "46005a82-a612-4dc1-9279-7215df6895cd"
        },
        "solution": {
          "solutionSubject": "Operate eye disease.",
          "investigation": "Diseases on the left eye and abnormal eye development and function.",
          "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
        },
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {
          "firstName": "Katherine",
          "lastName": "Marshall",
          "phone": 8452877665,
          "email": "kathmarshall@hm.io",
          "id": "26005a82-a612-4dc1-9279-7215df6895cd",
          "assignedOn": "2021-03-30T08:30:00Z",
          "profession": "Ophthalmologists"
        },
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          }
        ]
      },
      {
        "status": "Active",
        "category": "Eye",
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientDetail": {
          "firstName": "Matt",
          "lastName": "Turner",
          "userName": "mattturner10",
          "phone": 9452877662,
          "email": "mattturner@gmail.com",
          "id": "46005a82-a612-4dc1-9279-7215df6895cd"
        },
        "solution": {
          "solutionSubject": "Operate eye disease.",
          "investigation": "Diseases on the left eye and abnormal eye development and function.",
          "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
        },
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {
          "firstName": "Katherine",
          "lastName": "Marshall",
          "phone": 8452877665,
          "email": "kathmarshall@hm.io",
          "id": "26005a82-a612-4dc1-9279-7215df6895cd",
          "assignedOn": "2021-03-30T08:30:00Z",
          "profession": "Ophthalmologists"
        },
        "milestones": [
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          },
          {
            "description": "Home therapy for left eye before surgery.",
            "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
            "createdAt": "2022-10-21T01:12:23.926Z"
          }
        ],
        "activities": [
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
            "createdAt": "2022-10-21T01:14:27.516Z"
          },
          {
            "description": "Uploaded X-Ray report.",
            "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
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
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



***Status Code:*** 400

<br>



#### III. Example Request: Not found.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



***Status Code:*** 404

<br>



#### IV. Example Request: Internal Server Error. Please try again later.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



***Status Code:*** 500

<br>



## cases



### 1. {id}



***Endpoint:***

```bash
Method: 
Type: 
URL: 
```



### 2. Create a case.


Create a new case using the input provided and add it to the system.


***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{baseUrl}}/cases
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| Accept | application/json |  |



***Body:***

```js        
{
  "status": "Active",
  "category": "Eye",
  "severity": "0-Critical Impact",
  "subject": "Operation follow-up",
  "patientDetail": {
    "firstName": "Matt",
    "lastName": "Turner",
    "userName": "mattturner10",
    "phone": 9452877662,
    "email": "mattturner@gmail.com",
    "id": "46005a82-a612-4dc1-9279-7215df6895cd"
  },
  "solution": {
    "solutionSubject": "Operate eye disease.",
    "investigation": "Diseases on the left eye and abnormal eye development and function.",
    "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
  },
  "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
  "createdAt": "2021-03-30T08:30:00Z",
  "modifiedAt": "2021-04-28T08:30:00Z",
  "assignedTo": {
    "firstName": "Katherine",
    "lastName": "Marshall",
    "phone": 8452877665,
    "email": "kathmarshall@hm.io",
    "id": "26005a82-a612-4dc1-9279-7215df6895cd",
    "assignedOn": "2021-03-30T08:30:00Z",
    "profession": "Ophthalmologists"
  },
  "milestones": [
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    },
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    }
  ],
  "activities": [
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    },
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    }
  ]
}
```



***More example Requests/Responses:***


#### I. Example Request: Successfully created case.



***Body:***

```js        
{
  "status": "Active",
  "category": "Eye",
  "severity": "0-Critical Impact",
  "subject": "Operation follow-up",
  "patientDetail": {
    "firstName": "Matt",
    "lastName": "Turner",
    "userName": "mattturner10",
    "phone": 9452877662,
    "email": "mattturner@gmail.com",
    "id": "46005a82-a612-4dc1-9279-7215df6895cd"
  },
  "solution": {
    "solutionSubject": "Operate eye disease.",
    "investigation": "Diseases on the left eye and abnormal eye development and function.",
    "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
  },
  "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
  "createdAt": "2021-03-30T08:30:00Z",
  "modifiedAt": "2021-04-28T08:30:00Z",
  "assignedTo": {
    "firstName": "Katherine",
    "lastName": "Marshall",
    "phone": 8452877665,
    "email": "kathmarshall@hm.io",
    "id": "26005a82-a612-4dc1-9279-7215df6895cd",
    "assignedOn": "2021-03-30T08:30:00Z",
    "profession": "Ophthalmologists"
  },
  "milestones": [
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    },
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    }
  ],
  "activities": [
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    },
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    }
  ]
}
```



#### I. Example Response: Successfully created case.
```js
{
  "status": "Active",
  "category": "Eye",
  "severity": "0-Critical Impact",
  "subject": "Operation follow-up",
  "patientDetail": {
    "firstName": "Matt",
    "lastName": "Turner",
    "userName": "mattturner10",
    "phone": 9452877662,
    "email": "mattturner@gmail.com",
    "id": "46005a82-a612-4dc1-9279-7215df6895cd"
  },
  "solution": {
    "solutionSubject": "Operate eye disease.",
    "investigation": "Diseases on the left eye and abnormal eye development and function.",
    "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
  },
  "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
  "createdAt": "2021-03-30T08:30:00Z",
  "modifiedAt": "2021-04-28T08:30:00Z",
  "assignedTo": {
    "firstName": "Katherine",
    "lastName": "Marshall",
    "phone": 8452877665,
    "email": "kathmarshall@hm.io",
    "id": "26005a82-a612-4dc1-9279-7215df6895cd",
    "assignedOn": "2021-03-30T08:30:00Z",
    "profession": "Ophthalmologists"
  },
  "milestones": [
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    },
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    }
  ],
  "activities": [
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    },
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
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
  "status": "Active",
  "category": "Eye",
  "severity": "0-Critical Impact",
  "subject": "Operation follow-up",
  "patientDetail": {
    "firstName": "Matt",
    "lastName": "Turner",
    "userName": "mattturner10",
    "phone": 9452877662,
    "email": "mattturner@gmail.com",
    "id": "46005a82-a612-4dc1-9279-7215df6895cd"
  },
  "solution": {
    "solutionSubject": "Operate eye disease.",
    "investigation": "Diseases on the left eye and abnormal eye development and function.",
    "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
  },
  "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
  "createdAt": "2021-03-30T08:30:00Z",
  "modifiedAt": "2021-04-28T08:30:00Z",
  "assignedTo": {
    "firstName": "Katherine",
    "lastName": "Marshall",
    "phone": 8452877665,
    "email": "kathmarshall@hm.io",
    "id": "26005a82-a612-4dc1-9279-7215df6895cd",
    "assignedOn": "2021-03-30T08:30:00Z",
    "profession": "Ophthalmologists"
  },
  "milestones": [
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    },
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    }
  ],
  "activities": [
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    },
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
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
  "status": "Active",
  "category": "Eye",
  "severity": "0-Critical Impact",
  "subject": "Operation follow-up",
  "patientDetail": {
    "firstName": "Matt",
    "lastName": "Turner",
    "userName": "mattturner10",
    "phone": 9452877662,
    "email": "mattturner@gmail.com",
    "id": "46005a82-a612-4dc1-9279-7215df6895cd"
  },
  "solution": {
    "solutionSubject": "Operate eye disease.",
    "investigation": "Diseases on the left eye and abnormal eye development and function.",
    "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
  },
  "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
  "createdAt": "2021-03-30T08:30:00Z",
  "modifiedAt": "2021-04-28T08:30:00Z",
  "assignedTo": {
    "firstName": "Katherine",
    "lastName": "Marshall",
    "phone": 8452877665,
    "email": "kathmarshall@hm.io",
    "id": "26005a82-a612-4dc1-9279-7215df6895cd",
    "assignedOn": "2021-03-30T08:30:00Z",
    "profession": "Ophthalmologists"
  },
  "milestones": [
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    },
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    }
  ],
  "activities": [
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    },
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
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
  "status": "Active",
  "category": "Eye",
  "severity": "0-Critical Impact",
  "subject": "Operation follow-up",
  "patientDetail": {
    "firstName": "Matt",
    "lastName": "Turner",
    "userName": "mattturner10",
    "phone": 9452877662,
    "email": "mattturner@gmail.com",
    "id": "46005a82-a612-4dc1-9279-7215df6895cd"
  },
  "solution": {
    "solutionSubject": "Operate eye disease.",
    "investigation": "Diseases on the left eye and abnormal eye development and function.",
    "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
  },
  "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
  "createdAt": "2021-03-30T08:30:00Z",
  "modifiedAt": "2021-04-28T08:30:00Z",
  "assignedTo": {
    "firstName": "Katherine",
    "lastName": "Marshall",
    "phone": 8452877665,
    "email": "kathmarshall@hm.io",
    "id": "26005a82-a612-4dc1-9279-7215df6895cd",
    "assignedOn": "2021-03-30T08:30:00Z",
    "profession": "Ophthalmologists"
  },
  "milestones": [
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    },
    {
      "description": "Home therapy for left eye before surgery.",
      "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
      "createdAt": "2022-10-21T01:12:23.926Z"
    }
  ],
  "activities": [
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    },
    {
      "description": "Uploaded X-Ray report.",
      "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
      "createdAt": "2022-10-21T01:14:27.516Z"
    }
  ]
}
```



***Status Code:*** 500

<br>



### 3. Find all cases.


Get all the cases recorded in the system.


***Endpoint:***

```bash
Method: GET
Type: 
URL: {{baseUrl}}/cases
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 | Page number to paginate. |
| perPage | 10 | Total items to retrive at once. |



***More example Requests/Responses:***


#### I. Example Request: Successfully retrieved all the cases.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



#### I. Example Response: Successfully retrieved all the cases.
```js
[
  {
    "status": "Active",
    "category": "Eye",
    "severity": "0-Critical Impact",
    "subject": "Operation follow-up",
    "patientDetail": {
      "firstName": "Matt",
      "lastName": "Turner",
      "userName": "mattturner10",
      "phone": 9452877662,
      "email": "mattturner@gmail.com",
      "id": "46005a82-a612-4dc1-9279-7215df6895cd"
    },
    "solution": {
      "solutionSubject": "Operate eye disease.",
      "investigation": "Diseases on the left eye and abnormal eye development and function.",
      "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
    },
    "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
    "createdAt": "2021-03-30T08:30:00Z",
    "modifiedAt": "2021-04-28T08:30:00Z",
    "assignedTo": {
      "firstName": "Katherine",
      "lastName": "Marshall",
      "phone": 8452877665,
      "email": "kathmarshall@hm.io",
      "id": "26005a82-a612-4dc1-9279-7215df6895cd",
      "assignedOn": "2021-03-30T08:30:00Z",
      "profession": "Ophthalmologists"
    },
    "milestones": [
      {
        "description": "Home therapy for left eye before surgery.",
        "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
        "createdAt": "2022-10-21T01:12:23.926Z"
      },
      {
        "description": "Home therapy for left eye before surgery.",
        "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
        "createdAt": "2022-10-21T01:12:23.926Z"
      }
    ],
    "activities": [
      {
        "description": "Uploaded X-Ray report.",
        "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
        "createdAt": "2022-10-21T01:14:27.516Z"
      },
      {
        "description": "Uploaded X-Ray report.",
        "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
        "createdAt": "2022-10-21T01:14:27.516Z"
      }
    ]
  },
  {
    "status": "Active",
    "category": "Eye",
    "severity": "0-Critical Impact",
    "subject": "Operation follow-up",
    "patientDetail": {
      "firstName": "Matt",
      "lastName": "Turner",
      "userName": "mattturner10",
      "phone": 9452877662,
      "email": "mattturner@gmail.com",
      "id": "46005a82-a612-4dc1-9279-7215df6895cd"
    },
    "solution": {
      "solutionSubject": "Operate eye disease.",
      "investigation": "Diseases on the left eye and abnormal eye development and function.",
      "resolution": "Successfully operate on disease on the left eye and normal eye development and function."
    },
    "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
    "createdAt": "2021-03-30T08:30:00Z",
    "modifiedAt": "2021-04-28T08:30:00Z",
    "assignedTo": {
      "firstName": "Katherine",
      "lastName": "Marshall",
      "phone": 8452877665,
      "email": "kathmarshall@hm.io",
      "id": "26005a82-a612-4dc1-9279-7215df6895cd",
      "assignedOn": "2021-03-30T08:30:00Z",
      "profession": "Ophthalmologists"
    },
    "milestones": [
      {
        "description": "Home therapy for left eye before surgery.",
        "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
        "createdAt": "2022-10-21T01:12:23.926Z"
      },
      {
        "description": "Home therapy for left eye before surgery.",
        "id": "30027811-1ddb-4135-bb94-3a68aae1491c",
        "createdAt": "2022-10-21T01:12:23.926Z"
      }
    ],
    "activities": [
      {
        "description": "Uploaded X-Ray report.",
        "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
        "createdAt": "2022-10-21T01:14:27.516Z"
      },
      {
        "description": "Uploaded X-Ray report.",
        "id": "a7a32579-d7c3-45ef-8b5f-8eac996db599",
        "createdAt": "2022-10-21T01:14:27.516Z"
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
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



***Status Code:*** 400

<br>



#### III. Example Request: Not found.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



***Status Code:*** 404

<br>



#### IV. Example Request: Internal Server Error. Please try again later.



***Query:***

| Key | Value | Description |
| --- | ------|-------------|
| page | 1 |  |
| perPage | 10 |  |



***Body: None***



***Status Code:*** 500

<br>



---
[Back to top](#case-manager-api-collection)

>Generated at 2022-10-24 18:22:51 by [docgen](https://github.com/thedevsaddam/docgen)
