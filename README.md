# TD SYNNEX

TD SYNNEX is one of the world's largest IT distributors and solutions aggregators, serving over 150,000 resellers, retailers, and other customers in more than 100 countries. The company provides technology distribution, integration, and solutions services. TD SYNNEX offers the StreamOne Ion platform with REST APIs enabling partners to manage cloud subscriptions, customers, orders, and billing through a unified interface supporting multiple cloud vendors.

**Website:** [https://www.tdsynnex.com/na/us/](https://www.tdsynnex.com/na/us/)  
**API Documentation:** [https://docs.streamone.cloud/](https://docs.streamone.cloud/)  
**API Portal:** [https://www.tdsynnex.com/ion/api/](https://www.tdsynnex.com/ion/api/)

## APIs

### TD SYNNEX StreamOne Ion Partner API

The StreamOne Ion Partner API provides partners with programmatic access to TD SYNNEX cloud distribution services. Enables management of end customers, product catalogs, orders, subscriptions, shopping carts, and reporting.

- **Base URL:** `https://ion.tdsynnex.com`
- **Authentication:** OAuth 2.0
- **OpenAPI:** [openapi/td-synnex-streamone-ion-openapi.yml](openapi/td-synnex-streamone-ion-openapi.yml)

#### Key Endpoints

| Method | Path | Summary |
|--------|------|---------|
| POST | `/oauth/token` | Get Access Token |
| GET | `/v3/accounts/{accountId}/customers` | List Customers |
| POST | `/v3/accounts/{accountId}/customers` | Create Customer |
| GET | `/v3/accounts/{accountId}/products` | List Products |
| GET | `/v3/accounts/{accountId}/orders` | List Orders |
| POST | `/v3/accounts/{accountId}/orders` | Create Order |
| GET | `/v3/accounts/{accountId}/customers/{customerId}/subscriptions` | List Customer Subscriptions |
| POST | `/v3/accounts/{accountId}/customers/{customerId}/carts` | Create Cart |
| POST | `/v3/accounts/{accountId}/customers/{customerId}/carts/{cartId}/checkout` | Checkout Cart |
| GET | `/v3/accounts/{accountId}/reports/{reportId}/data` | Get Report Data |

## Features

- **Customer Management** - Create, retrieve, update, and manage end customer accounts
- **Product Catalog** - Browse technology products from multiple vendors
- **Order Management** - Create, update, and manage product orders
- **Subscription Management** - Track and manage cloud software subscriptions
- **Shopping Cart** - Staged ordering workflow with cart checkout
- **Cloud Provider Integration** - Link customer accounts to cloud providers
- **Business Intelligence Reports** - Access distribution analytics and reporting
- **Multi-Vendor Support** - Single interface for multiple cloud vendors
- **OAuth 2.0** - Secure authentication with refresh token flow

## Use Cases

- **MSP Subscription Management** - Automate cloud subscription billing and management
- **Reseller Order Automation** - Automate technology product ordering workflows
- **Cloud Marketplace Integration** - Integrate TD SYNNEX into custom partner portals
- **Customer Lifecycle Management** - End-to-end customer provisioning automation
- **Business Intelligence** - Pull reporting data into custom analytics platforms

## Artifacts

### OpenAPI Specifications

| File | Description |
|------|-------------|
| [openapi/td-synnex-streamone-ion-openapi.yml](openapi/td-synnex-streamone-ion-openapi.yml) | StreamOne Ion Partner API |

### Naftiko Capabilities

| File | Description |
|------|-------------|
| [capabilities/cloud-distribution.yaml](capabilities/cloud-distribution.yaml) | Cloud distribution lifecycle management workflow |
| [capabilities/shared/streamone-ion.yaml](capabilities/shared/streamone-ion.yaml) | Shared StreamOne Ion API definition |

### Spectral Rules

| File | Description |
|------|-------------|
| [rules/td-synnex-rules.yml](rules/td-synnex-rules.yml) | Spectral ruleset for TD SYNNEX API conventions |

### JSON Schemas

| File | Description |
|------|-------------|
| [json-schema/td-synnex-customer-schema.json](json-schema/td-synnex-customer-schema.json) | End customer account schema |
| [json-schema/td-synnex-order-schema.json](json-schema/td-synnex-order-schema.json) | Technology product order schema |

### JSON Structures

| File | Description |
|------|-------------|
| [json-structure/td-synnex-customer-structure.json](json-structure/td-synnex-customer-structure.json) | Customer field documentation |

### JSON-LD Context

| File | Description |
|------|-------------|
| [json-ld/td-synnex-context.jsonld](json-ld/td-synnex-context.jsonld) | Linked data context for distribution vocabulary |

### Examples

| File | Description |
|------|-------------|
| [examples/td-synnex-create-customer-example.json](examples/td-synnex-create-customer-example.json) | Create end customer example |
| [examples/td-synnex-create-order-example.json](examples/td-synnex-create-order-example.json) | Create product order example |

### Vocabulary

| File | Description |
|------|-------------|
| [vocabulary/td-synnex-vocabulary.yml](vocabulary/td-synnex-vocabulary.yml) | Technology distribution domain terminology |

## Integrations

- **Microsoft** - Azure and Microsoft 365 cloud subscription distribution
- **AWS** - Amazon Web Services subscription management
- **Google Cloud** - Google Cloud Platform subscription management
- **Rewst** - Workflow automation integration

## Maintainers

**FN:** Kin Lane  
**Email:** info@apievangelist.com
