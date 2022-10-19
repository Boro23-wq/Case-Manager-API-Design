## Case Manager API Collection
The API performs CRUD operation on case managers. The API is part of the project CS 673 - Care Management and Co-ordination.

**Contact Support:**
Name: Sintu Boro  
Email: [sb394@njit.edu](mailto:sb394@njit.edu)
Url: [sboro.vercel.app](https://sboro.vercel.app/)

---

#### PATH - /caseManagers

**POST** - Create a case manager.
```http://localhost:3000/caseManagers```
Creates a new case manager using the required fields and adds it to the system.

**Request Headers:**
***Content-Type*** - application/json
***Accept*** - application/json

**Body raw  (json):**
```json
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}
```

**Example Request:**
```cURL
curl --location --request POST 'http://localhost:3000/caseManagers' \
--header 'Content-Type: application/json' \
--header 'Accept: application/json' \
--data-raw '{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}'
```
**Response Body**:
```json
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}
```

**GET** - Find all case managers.
```http://localhost:3000/caseManagers```
Get all the case managers and their cases.

**Request Headers:**
***Accept*** - application/json

**Example Request:**
```cURL
curl --location --request GET 'http://localhost:3000/caseManagers' \
--header 'Accept: application/json'
```

**Response Body:**
```json
[
  {
    "username": "johndoe",
    "firstName": "John",
    "lastName": "Doe",
    "email": "johndoe@cm.io",
    "phone": 8623817665,
    "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
    "createdAt": "2021-01-30T08:30:00Z",
    "modifiedAt": "2021-01-31T08:30:00Z",
    "cases": [
      {
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
      },
      {
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
      }
    ]
  },
  {
    "username": "johndoe",
    "firstName": "John",
    "lastName": "Doe",
    "email": "johndoe@cm.io",
    "phone": 8623817665,
    "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
    "createdAt": "2021-01-30T08:30:00Z",
    "modifiedAt": "2021-01-31T08:30:00Z",
    "cases": [
      {
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
      },
      {
        "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
        "createdAt": "2021-03-30T08:30:00Z",
        "modifiedAt": "2021-04-28T08:30:00Z",
        "assignedTo": {},
        "severity": "0-Critical Impact",
        "subject": "Operation follow-up",
        "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
      }
    ]
  }
]
```

---

#### PATH - /caseManager/{id}

**GET** - Find case manager by ID.
```http://localhost:3000/caseManager/:id```
Returns a single case manager

**Request Headers:**
***Accept*** - application/json

**Example Request:**

```cURL
curl --location --request GET 'http://localhost:3000/caseManager/66168742' \
--header 'Accept: application/json'
```

**Response Body:**

```json
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}
```

**PUT** - Update a case manager.
```http://localhost:3000/caseManager/:id```
Update details of a case manager with the ID.

**Request Headers:**
***Content-Type*** - application/json
***Accept*** - application/json

**Path Variables:**
****id*** - (Required) The id of the case manager that needs to be updated

**Body raw (json):**
```json
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}
```

**Example Request:**

```cURL
curl --location --request PUT 'http://localhost:3000/caseManager/66168742' \
--header 'Content-Type: application/json' \
--header 'Accept: application/json' \
--data-raw '{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}'
```

**Response Body:**

```json
{
  "username": "johndoe",
  "firstName": "John",
  "lastName": "Doe",
  "email": "johndoe@cm.io",
  "phone": 8623817665,
  "id": "378cdddc-31af-481c-9000-2ab4eabeebaf",
  "createdAt": "2021-01-30T08:30:00Z",
  "modifiedAt": "2021-01-31T08:30:00Z",
  "cases": [
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    },
    {
      "caseId": "36005a82-a612-4dc1-9279-7215df6895cd",
      "createdAt": "2021-03-30T08:30:00Z",
      "modifiedAt": "2021-04-28T08:30:00Z",
      "assignedTo": {},
      "severity": "0-Critical Impact",
      "subject": "Operation follow-up",
      "patientID": "6c47da92-4b6a-431c-8cbe-78f8d386625f"
    }
  ]
}
```

**DELETE** - Delete a case manager.
```http://localhost:3000/caseManager/:id```
Delete an existing case manager.

**Request Headers:**
***Accept*** - application/json

**Path Variables:**
****id*** - (Required) The id of the case manager that needs to be updated

**Example Request:**
```cURL
curl --location --request DELETE 'http://localhost:3000/caseManager/66168742' \
--header 'Accept: application/json'
```

**Response Body:**
```json
"290cdddc-31af-481c-9000-2ab4eabeebaf"
```