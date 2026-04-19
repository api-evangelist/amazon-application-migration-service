# Amazon Application Migration Service

AWS Application Migration Service (MGN) is the primary migration service recommended for lift-and-shift migrations to AWS. It allows organizations to quickly realize the benefits of migrating applications to the cloud without changes and with minimal downtime.

## Overview

The Amazon Application Migration Service API provides programmatic control over source server registration, continuous replication, test and cutover operations, and post-migration management. It enables automated lift-and-shift migrations with minimal downtime.

## API Documentation

- **Human URL:** https://docs.aws.amazon.com/mgn/latest/APIReference/Welcome.html
- **Base URL:** https://mgn.us-east-1.amazonaws.com

## Features

- Continuous block-level replication with near-zero RPO
- Automated lift-and-shift migration without application changes
- Test migration capability without impacting production servers
- Wave and application grouping for phased migration management
- Agentless migration via VMware vCenter connector
- Post-launch automation via AWS Systems Manager documents
- Right-sizing recommendations for target instance types
- Cross-account and cross-region migration support
- Integration with AWS Migration Hub for centralized tracking
- Automatic EC2 launch template creation for migrated servers

## Use Cases

- Migrate on-premises data center servers to AWS with minimal downtime
- Execute phased migrations organized by application waves
- Test migration outcomes before executing production cutover
- Migrate VMware virtual machines to EC2 instances without agent installation
- Standardize migration configuration across hundreds of servers with templates
- Automate post-migration software installation and configuration with SSM

## Artifacts

### OpenAPI Specification
`openapi/amazon-application-migration-service-openapi.yml`

Complete OpenAPI 3.1.0 specification covering all 40 API paths including source servers, replication, launch, jobs, applications, waves, and tags.

### Spectral Rules
`rules/amazon-application-migration-service-spectral-rules.yml`

Linting rules for validating OpenAPI specifications for this service.

### Naftiko Capabilities
- `capabilities/shared/application-migration-service-api.yaml` — Shared per-API capability definition
- `capabilities/lift-and-shift-migration.yaml` — Workflow capability for lift-and-shift migration use cases

### Vocabulary
`vocabulary/amazon-application-migration-service-vocabulary.yaml`

Structured vocabulary of resources, actions, workflows, and personas.

### JSON Schemas
`json-schema/` — 100 JSON Schema draft/2020-12 files for all request and response objects.

### JSON Structures
`json-structure/` — 100 JSON Structure files for all objects.

### JSON-LD Context
`json-ld/amazon-application-migration-service-context.jsonld`

### Examples
`examples/` — 100 example JSON files for all objects.

## Integrations

- AWS Migration Hub
- Amazon EC2
- Amazon EBS
- AWS Systems Manager
- VMware vCenter
- AWS IAM
- Amazon CloudWatch
- AWS CloudTrail
- Amazon S3
- AWS KMS

## Tags

Amazon Application Migration Service, Migration, Lift And Shift, AWS, Cloud Migration

## Maintainers

- Kin Lane (kin@apievangelist.com)
