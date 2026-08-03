# Amazon Application Migration Service

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
