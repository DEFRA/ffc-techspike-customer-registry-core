# ffc-techspike-customer-registry-core
Local development support for orchestrating all FFC customer registry microservices with Docker Compose.

## Prerequisites

Ensure you have satisfied the prerequisites of all individual repositories.

## Customer registry microservices
### Customer registry graphql api

Query data from both the Azre cognitive service and Azure cosmosdb with the grahql.

- https://github.com/DEFRA/ffc-techspike-customer-registry

### Customer registry web

Frontend service integrated with the customer registry graphql api.

- https://github.com/DEFRA/ffc-techspike-customer-registry-web

### Customer registery data consumer

Consuming data sent to an event queue. Data is processed and save to an Azure cosmosdb

- https://github.com/DEFRA/ffc-techspike-customer-registry-data-consumer

### Customer registery event

consuming events sent to the Customer registery data consumer. Events are saved to an Azure Blob table

- https://github.com/DEFRA/ffc-techspike-customer-registry-event

### Customer registery alert

Integrated with gov notify to send alerts via emails.

- https://github.com/DEFRA/ffc-techspike-customer-registry-alert
