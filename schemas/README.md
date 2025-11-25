# GS1 Verifiable Credential JSON Schemas

This directory contains JSON Schema definitions for GS1 Verifiable Credentials.

## Schema Types

### License and Key Credentials (Strict Validation)
- **gs1-prefix-schema.json** - GS1 Prefix License issued by GS1 Global Office
- **gs1-company-prefix-schema.json** - GS1 Company Prefix License issued by GS1 Member Organizations
- **gs1-key-schema.json** - Key Credential for GS1 identified entities
- **gs1-product-key-schema.json** - Product Key Credential

These schemas use strict `const` validation to enforce exact credential types.

### Data Credentials (Flexible Validation)
- **gs1-organization-data-schema.json** - Organization Data Credential
- **gs1-product-data-schema.json** - Product Data Credential

These schemas use flexible validation with required `contains` constraints, allowing for credential type extensions while ensuring core types are always present.
This allows to potentially extend data holding credentials while licenses and keys must strictly follow the data model.

## Validation Approach

All schemas comply with [JSON Schema Draft 2020-12](https://json-schema.org/draft/2020-12/schema) and enforce W3C Verifiable Credentials v2 standards.

