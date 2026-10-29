# Data model

All table and column names in this document are fictional.

## Service Request (`nsg_servicerequest`)

| Column | Type | Description | Notes |
| --- | --- | --- | --- |
| `nsg_requestnumber` | Autonumber | Human-readable request identifier. | Example: `SR-1042`. |
| `nsg_title` | Text | Short description of the incoming request. | Required. |
| `nsg_requesteremail` | Email | E-mail address supplied by the requester. | Required for the automatic confirmation. |
| `nsg_servicecategory` | Choice | Category selected by the coordinator. | See `source-material/Service-catalog.md`. |
| `nsg_priority` | Choice | Business priority: Low, Normal, High. | Default is Normal. |
| `nsg_status` | Choice | Lifecycle state of the request. | See `features/onboarding-guide/Workflow.md`. |
| `nsg_assignedteam` | Lookup | Service team responsible for handling the request. | Required before status becomes In progress. |
| `nsg_assetreference` | Lookup | Related reference asset, when supplied. | Optional. |

## Service Update (`nsg_serviceupdate`)

A Service Update is a child record used by service teams to record a meaningful status update. It is not required for request registration.

| Column | Type | Description |
| --- | --- | --- |
| `nsg_servicerequest` | Lookup | Parent Service Request. |
| `nsg_updatecomment` | Multiline text | Internal update. |
| `nsg_visibletorequester` | Yes/No | Whether the text can be used in a customer update. |

## Relationship summary

- One Service Request can have many Service Updates.
- One Service Team can own many Service Requests.
- An Asset Reference can be associated with many Service Requests.

## Training note

The guide should use business-friendly names such as **Service Request** rather than logical table names unless the specification explicitly asks for technical detail.
