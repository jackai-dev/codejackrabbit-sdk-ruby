# CodeJackRabbit Ruby API

<!-- omniwrap-api-reference eyJjb250cmFjdF9maW5nZXJwcmludCI6ImIwNjc4MWEyNmM0NDY5ZThmMTI4MzBhMDRkNDU1OTU3YmY2MjBkNDJiOWUxZGYxNTVlOTNlZTAwZjI5M2QxYzkiLCJvcGVyYXRpb25fY291bnQiOjI4LCJyZW5kZXJlciI6InJ1YnkiLCJ2ZXJzaW9uIjoiMS41LjAifQ -->

This generated index is tied to Semantic IR `1.14.0` and contract fingerprint `b06781a26c4469e8f12830a04d455957bf620d42b9e1df155e93ee00f293d1c9`. Every operation below is rendered from the same semantic contract and artifact-attested public member allocation as the SDK.

SDK maturity: **experimental**  
Artifact evidence: [`omniwrap-artifact.json`](omniwrap-artifact.json) binds this file by SHA-256 and is revalidated by the package gate.

## Shared types

- `AuditContextRequest`
- `AuditSnapshotsRequest`
- `ComplianceGateRequest`
- `DeveloperAuditRequest`
- `DeveloperEvidenceRequest`
- `FileChange`
- `FinOpsRequest`
- `ManagedDeveloperIdentity`
- `ManagedDeveloperIdentityRequest`
- `ReviewRequest`
- `WaitlistRequest`

## Resource `analysis`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJhbmFseXplX2NvbnRyYWN0X2RyaWZ0IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImFuYWx5emVDb250cmFjdERyaWZ0IiwicGF0aCI6Ii92MS9hbmFseXNpcy9jb250cmFjdC1kcmlmdCIsInJlc291cmNlIjoiYW5hbHlzaXMiLCJzZWN0aW9uX3NoYTI1NiI6Ijg4MzFmNTg5MDVkOGQ5NTA2YWEyOTE4MTdmM2JlZWQ0M2Y3MDEwNzBlODE2YWIwMjc3MTRkZDZlYjM2ZmMwNDgiLCJzaWduYXR1cmVfc2hhMjU2IjoiZWVjNjg2ZTUzMDg4MTFkZDI1YTEyZmU0NjViZGQ4YmNhM2JhNmY3MzA3MmNiNjNiMzQ5MjNhZGVmM2YyMjc3YiJ9 -->
### `client.analyze_contract_drift`

Operation ID: `analyzeContractDrift`  
Route: `POST` `/v1/analysis/contract-drift`  

#### Signature

```ruby
def analyze_contract_drift(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Contract drift report and SemVer recommendation | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJhbmFseXplQ29udHJhY3REcmlmdCJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJhbmFseXplX3BlcmZfZmluX29wcyIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJhbmFseXplUGVyZkZpbk9wcyIsInBhdGgiOiIvdjEvYW5hbHlzaXMvcGVyZi1maW5vcHMiLCJyZXNvdXJjZSI6ImFuYWx5c2lzIiwic2VjdGlvbl9zaGEyNTYiOiIzN2QxMThkNTE3MzMxODQwYmQyYzc0NDY3ZjJiMDQ1NzRkOWM2N2MzZTliNjNiODc5MzFiNTAyNTA4ZDYyODVhIiwic2lnbmF0dXJlX3NoYTI1NiI6IjQwM2RiOWRjOTQzZDVhOGExZDI1OWQ1NTQwMGZlODY1ZWQ5ZDQ2MGY2YTQyZDE2YThmNTVkZGFiYzA0YjcwZWMifQ -->
### `client.analyze_perf_fin_ops`

Operation ID: `analyzePerfFinOps`  
Route: `POST` `/v1/analysis/perf-finops`  

#### Signature

```ruby
def analyze_perf_fin_ops(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Performance and FinOps audit report | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJhbmFseXplUGVyZkZpbk9wcyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJwbGFuX3N0YWNrZWRfcHJfc3BsaXQiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoicGxhblN0YWNrZWRQclNwbGl0IiwicGF0aCI6Ii92MS9hbmFseXNpcy9zcGxpdC1wciIsInJlc291cmNlIjoiYW5hbHlzaXMiLCJzZWN0aW9uX3NoYTI1NiI6ImM3ZmQzOWE4NWFmZWEyZDk2NWI0NGZkYTM4MDhhZmY3MzI2ODUyODIxMjg1YzMxNjhiMTI2YjlhZjE3NDI1NzEiLCJzaWduYXR1cmVfc2hhMjU2IjoiZTI0ZjQ4YzM2MTQyOGE1MTlmYWY3NmU1YWEyMDBmYzk3ZjExNzZmZjk2Yjk1MDBlNjM4OThhZTRmYWY0NzBjMSJ9 -->
### `client.plan_stacked_pr_split`

Operation ID: `planStackedPrSplit`  
Route: `POST` `/v1/analysis/split-pr`  

#### Signature

```ruby
def plan_stacked_pr_split(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Ordered stacked PR plan and git commands | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJwbGFuU3RhY2tlZFByU3BsaXQifQ -->

## Resource `analytics`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYW5hbHl0aWNzX3JvaSIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6ImdldEFuYWx5dGljc1JvaSIsInBhdGgiOiIvdjEvYW5hbHl0aWNzL3JvaSIsInJlc291cmNlIjoiYW5hbHl0aWNzIiwic2VjdGlvbl9zaGEyNTYiOiJiYjk5NTc0ZjM1OWUxZWUwZmM4YTU3OGNhYmJjNzQzNjE1NDQwMzFjZTA5ZTQ1NzZkMzI2N2I3ZGQzYWNmNmI5Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjQxM2VlODdlM2MwMzRjMmNlZDkwYTMxMWYxYmM3MzlmY2ExZjhiZGMyMjY1MTllZjhhYTU5MWI1OTg3NDJhODIifQ -->
### `client.get_analytics_roi`

Operation ID: `getAnalyticsRoi`  
Route: `GET` `/v1/analytics/roi`  

#### Signature

```ruby
def get_analytics_roi()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | ROI telemetry summary | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRBbmFseXRpY3NSb2kifQ -->

## Resource `capabilities`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfY2FwYWJpbGl0aWVzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0Q2FwYWJpbGl0aWVzIiwicGF0aCI6Ii92MS9jYXBhYmlsaXRpZXMiLCJyZXNvdXJjZSI6ImNhcGFiaWxpdGllcyIsInNlY3Rpb25fc2hhMjU2IjoiNDc2NGQ1MDAyZTg1NjY1YWY4ZDQyZDg1NWQ2YWMxZTcwODY5N2VkM2U4ZDA2NWVhNDY2OTkxZjEzZmI3Yjg1MiIsInNpZ25hdHVyZV9zaGEyNTYiOiJhZmVjZmVlNGYzMTQyNjUzMDAwNTRhNDVkZDMzNWI5NWYzMGFmMDg2MmI0MjI3OWIxN2UwODU4ZWFmMDljNWU2In0 -->
### `client.get_capabilities`

Operation ID: `getCapabilities`  
Route: `GET` `/v1/capabilities`  

#### Signature

```ruby
def get_capabilities()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Capabilities catalog | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRDYXBhYmlsaXRpZXMifQ -->

## Resource `compliance`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJldmFsdWF0ZV9jb21wbGlhbmNlX2dhdGUiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiZXZhbHVhdGVDb21wbGlhbmNlR2F0ZSIsInBhdGgiOiIvdjEvY29tcGxpYW5jZS9nYXRlIiwicmVzb3VyY2UiOiJjb21wbGlhbmNlIiwic2VjdGlvbl9zaGEyNTYiOiIxOGRlMWVjMTRjZGU3MGMxNWM2NGE1MTZiYjE5N2FlMTM2N2UwNDA0NmExYWQzYjVmNzdjNzUyNzlkNTBhODM0Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjU1ZmQ5ZTk0ZTc2NDY2YzlkNTM1NmVhNzI3YzgwOThjNWM3NGMwMzM1OTI4MmZhMDczNDllNGIyNzliYjU3NWMifQ -->
### `client.evaluate_compliance_gate`

Operation ID: `evaluateComplianceGate`  
Route: `POST` `/v1/compliance/gate`  

#### Signature

```ruby
def evaluate_compliance_gate(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ComplianceGateRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Compliance gate verdict and SHA-256 attestation | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJldmFsdWF0ZUNvbXBsaWFuY2VHYXRlIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJleHBvcnRfc2FyaWYiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiZXhwb3J0U2FyaWYiLCJwYXRoIjoiL3YxL2NvbXBsaWFuY2Uvc2FyaWYiLCJyZXNvdXJjZSI6ImNvbXBsaWFuY2UiLCJzZWN0aW9uX3NoYTI1NiI6ImM2ZDgyOGFjYzUwN2Q3NGQ3OTY4OGQ4ODdmMzE4YmYzOTQ0ZDllM2E1NDQ4YjE2OTE2NzczZTQ0MTY0ZDgxOGYiLCJzaWduYXR1cmVfc2hhMjU2IjoiNWI4ZWU3MDhjNWQ5YzdjZDQ2ZDkyMmU2YmI3MDQwOWVhYTdlZTMwYWE2ZWNiOWUyOTU5MTFlMTk5MTVjOGY1NyJ9 -->
### `client.export_sarif`

Operation ID: `exportSarif`  
Route: `POST` `/v1/compliance/sarif`  

#### Signature

```ruby
def export_sarif(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | SARIF 2.1.0 JSON document | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJleHBvcnRTYXJpZiJ9 -->

## Resource `developer_intelligence`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjb2xsZWN0X2RldmVsb3Blcl9hdWRpdCIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJjb2xsZWN0RGV2ZWxvcGVyQXVkaXQiLCJwYXRoIjoiL2NsaS9tYW5hZ2VkL2RldmVsb3Blci1hdWRpdCIsInJlc291cmNlIjoiZGV2ZWxvcGVyX2ludGVsbGlnZW5jZSIsInNlY3Rpb25fc2hhMjU2IjoiOGExZGI2MDllZmE3YmZmMTU4NzlkODM3YTU2ZDU5OWY2N2ZiZjliMTNjNTg1YmMzYjcwNjVmZGJhOTljMmIwMiIsInNpZ25hdHVyZV9zaGEyNTYiOiIyNTQxMDMwMjEwZGE0MDEwMWE4MmI1YjNjZTE3OWRjYjRjMWQwZjhmZWQzOWM0MjBjY2U2M2YzN2JhZGE0ZWFiIn0 -->
### `client.collect_developer_audit`

Operation ID: `collectDeveloperAudit`  
Route: `POST` `/cli/managed/developer-audit`  

#### Signature

```ruby
def collect_developer_audit(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `DeveloperAuditRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Versioned report with source coverage, missing evidence and immutable snapshot reference. | application/json (object) |
| `default` | Explicit authentication, paid access, source authorization, capacity or collection blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "from": "2026-01-09",
    "repositoryId": "1",
    "to": "2026-01-18"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjb2xsZWN0RGV2ZWxvcGVyQXVkaXQifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjdXJyZW50X2RldmVsb3Blcl9pZGVudGl0eSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJjdXJyZW50RGV2ZWxvcGVySWRlbnRpdHkiLCJwYXRoIjoiL2NsaS9tYW5hZ2VkL2RldmVsb3Blci1pZGVudGl0eSIsInJlc291cmNlIjoiZGV2ZWxvcGVyX2ludGVsbGlnZW5jZSIsInNlY3Rpb25fc2hhMjU2IjoiOWUyZjM4OTJlNGVlMDg1MTJmMmExMDU5MzYzMWFhZWMyNWViYjRiODFiYjA3MjE3ZjA0OGNmODMyNDkxZGM4YyIsInNpZ25hdHVyZV9zaGEyNTYiOiJhNmE3Y2YzZTFkMzNiZjcwN2Y1MzdiNDU5MjdkMmU0YjA2Mzk1ZWQyMTYxYzI3ZjRkYzQ5ODI4NmY1MmM2NDQyIn0 -->
### `client.current_developer_identity`

Operation ID: `currentDeveloperIdentity`  
Route: `POST` `/cli/managed/developer-identity`  

#### Signature

```ruby
def current_developer_identity(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ManagedDeveloperIdentityRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Current verified identity and authorized repositories. | application/json (ManagedDeveloperIdentity) |
| `default` | Explicit account, GitHub identity or source authorization blocker. | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjdXJyZW50RGV2ZWxvcGVySWRlbnRpdHkifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJkZWNsYXJlX2RldmVsb3Blcl9wcm9qZWN0X2NvbnRleHQiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiZGVjbGFyZURldmVsb3BlclByb2plY3RDb250ZXh0IiwicGF0aCI6Ii9jbGkvbWFuYWdlZC9hdWRpdC1jb250ZXh0IiwicmVzb3VyY2UiOiJkZXZlbG9wZXJfaW50ZWxsaWdlbmNlIiwic2VjdGlvbl9zaGEyNTYiOiI5MDQ3ZTQ1YmRjYWU4ZmE5MmM0YjVmYmRhMmQxNTRjZWZkMzU1MzhjY2Q2ZTM1ZGI3YjdiMTFhYmY5ODFlODExIiwic2lnbmF0dXJlX3NoYTI1NiI6IjRkYmExZTE0MmRiYmUyOWY4NzM0ZDFhYjc2ODkyNTQ3MWUxYjczM2IwOGE0OGFmZjE0NTZkYmM5MzM1ZDQ5NmUifQ -->
### `client.declare_developer_project_context`

Operation ID: `declareDeveloperProjectContext`  
Route: `POST` `/cli/managed/audit-context`  

#### Signature

```ruby
def declare_developer_project_context(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `AuditContextRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Immutable declaration or correction receipt. | application/json (object) |
| `default` | Explicit authorization, contributor identity, correction or storage capacity blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "declaration": {
      "contributorId": "1",
      "effectiveFrom": "2026-01-02",
      "effectiveTo": "2026-01-11",
      "snapshotId": "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
      "source": "example",
      "supersedes": "example",
      "type": "project_join",
      "value": "example"
    },
    "repositoryId": "1"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJkZWNsYXJlRGV2ZWxvcGVyUHJvamVjdENvbnRleHQifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJtYW5hZ2VkX2F1ZGl0X3NuYXBzaG90cyIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJtYW5hZ2VkQXVkaXRTbmFwc2hvdHMiLCJwYXRoIjoiL2NsaS9tYW5hZ2VkL2F1ZGl0LXNuYXBzaG90cyIsInJlc291cmNlIjoiZGV2ZWxvcGVyX2ludGVsbGlnZW5jZSIsInNlY3Rpb25fc2hhMjU2IjoiYjVhMTU5NmJhZGU5ZmU5YjBjMDBkNDQ5MDA3NGI3NDliOTMyYzAyNmIzMDEyNTE2MWEyN2QwM2Q2ZmFiMjJiZiIsInNpZ25hdHVyZV9zaGEyNTYiOiIzYTQyNDY5YTM5ODc2NzQ3N2U5Y2MzODlmYjQzMDA4MTBiOTRjNmNlMjRlYmJlMzhlYzVmMWFjNDNlZjljZmUzIn0 -->
### `client.managed_audit_snapshots`

Operation ID: `managedAuditSnapshots`  
Route: `POST` `/cli/managed/audit-snapshots`  

#### Signature

```ruby
def managed_audit_snapshots(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `AuditSnapshotsRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Snapshot list or digest-verified immutable envelope. | application/json (object) |
| `default` | Explicit authorization, expiry, missing snapshot or integrity blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "action": "list",
    "repositoryId": "1"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJtYW5hZ2VkQXVkaXRTbmFwc2hvdHMifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJwcm92aWRlcl9jb3N0X2V2aWRlbmNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InByb3ZpZGVyQ29zdEV2aWRlbmNlIiwicGF0aCI6Ii9jbGkvbWFuYWdlZC9maW5vcHMiLCJyZXNvdXJjZSI6ImRldmVsb3Blcl9pbnRlbGxpZ2VuY2UiLCJzZWN0aW9uX3NoYTI1NiI6IjYzYTc2NTYxZTk0MmJlZmU0YWQ3YjAyZDhiZTY4MWNmZDdhYzQ0Y2U2MzhhZTMwMWU0MmMyZjA0Y2ZjM2EzYmMiLCJzaWduYXR1cmVfc2hhMjU2IjoiYTI0NzJiMTVmZmNlNTgxYmM1M2E5YmEwZTFiYzU3NjBiNzJhOTQ3MmEwZTEzYTZlYWNiMjkzYWQ0NWNmMWUzYSJ9 -->
### `client.provider_cost_evidence`

Operation ID: `providerCostEvidence`  
Route: `POST` `/cli/managed/finops`  

#### Signature

```ruby
def provider_cost_evidence(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `FinOpsRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Server report or declaration receipt. Unknown costs remain null. | application/json (object) |
| `default` | Explicit permission, paid access, source or declaration validation blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "action": "report"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJwcm92aWRlckNvc3RFdmlkZW5jZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzdWJtaXRfZGV2ZWxvcGVyX2V2aWRlbmNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InN1Ym1pdERldmVsb3BlckV2aWRlbmNlIiwicGF0aCI6Ii9jbGkvbWFuYWdlZC9kZXZlbG9wZXItZXZpZGVuY2UiLCJyZXNvdXJjZSI6ImRldmVsb3Blcl9pbnRlbGxpZ2VuY2UiLCJzZWN0aW9uX3NoYTI1NiI6IjdlYzJiYTgyZDg4YjA4NWJjNzhiMTQ0Zjg1ZjA4OThjZDRiNGJhZmY2MTBhOGI1Nzc5Mjk4ZTg3Mzc1ZDgyZDIiLCJzaWduYXR1cmVfc2hhMjU2IjoiMjY0NDkyMTNmNTNhYTRjZTEwYzI2ZjllNzFjZDkwMGY2Y2IxM2UyZGZkYzM4Nzk2NGY4MDU3ZGNiYzQ4MTdmZiJ9 -->
### `client.submit_developer_evidence`

Operation ID: `submitDeveloperEvidence`  
Route: `POST` `/cli/managed/developer-evidence`  

#### Signature

```ruby
def submit_developer_evidence(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `DeveloperEvidenceRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Accepted and duplicate span counts. | application/json (object) |
| `default` | Explicit identity, repository, paid access or evidence validation blocker. | none |

#### Canonical required-input example

```json
{
  "body": {
    "category": "coding",
    "input": {},
    "repositoryId": "1"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdWJtaXREZXZlbG9wZXJFdmlkZW5jZSJ9 -->

## Resource `health`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfaGVhbHRoIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0SGVhbHRoIiwicGF0aCI6Ii9oZWFsdGgiLCJyZXNvdXJjZSI6ImhlYWx0aCIsInNlY3Rpb25fc2hhMjU2IjoiMDU1OWM4YzZjMzExOTUyODdiODZiYmVmYzdkNTQ5N2Q5NGU1Nzk1MzY0MDg5NzVhNjcyYWQ5MWFiNGVlODNiNyIsInNpZ25hdHVyZV9zaGEyNTYiOiIwMTVmZDY2MTBiYmU3OTRlYTUyZTNkNjZmMzZhODBjNWNlZTUxODlmOWE1NjU5OWRmYTUyNmM0Mjg0NTE3NjMxIn0 -->
### `client.get_health`

Operation ID: `getHealth`  
Route: `GET` `/health`  

#### Signature

```ruby
def get_health()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Server health status | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRIZWFsdGgifQ -->

## Resource `reviews`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJidWlsZF9hdXRvZml4X2J1bmRsZSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJidWlsZEF1dG9maXhCdW5kbGUiLCJwYXRoIjoiL3YxL3Jldmlld3MvYXV0b2ZpeCIsInJlc291cmNlIjoicmV2aWV3cyIsInNlY3Rpb25fc2hhMjU2IjoiM2YwZWY2OTA4MDNkOTc3YmE4ZmY0ODA0M2Y2YWMxZWQxYjg4ZGYxN2VjMTNmNjhmOTQwYWJmYjY3YmM5NDg3ZSIsInNpZ25hdHVyZV9zaGEyNTYiOiJmMzY5NGZmNGMxMzM3NWFmYzNmMjM2ZjhiMmU1MTcwNmQ0OGVjMDg3MTY5MTMxYWEyZTZiNDVmZGM1NDQ1ZjdhIn0 -->
### `client.build_autofix_bundle`

Operation ID: `buildAutofixBundle`  
Route: `POST` `/v1/reviews/autofix`  

#### Signature

```ruby
def build_autofix_bundle(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Remediation patch bundle | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJidWlsZEF1dG9maXhCdW5kbGUifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjb21wdXRlX3Jpc2tfcmFkYXIiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY29tcHV0ZVJpc2tSYWRhciIsInBhdGgiOiIvdjEvcmV2aWV3cy9yaXNrLXJhZGFyIiwicmVzb3VyY2UiOiJyZXZpZXdzIiwic2VjdGlvbl9zaGEyNTYiOiJiOWIzNjkwNDk5YjM5YzkyNzMxZTYxOTU3N2E0YjE2OWFjZmI5YzQ3NmFjNzI2OGY5OWRmYmM4ZDY5YzBhMjRhIiwic2lnbmF0dXJlX3NoYTI1NiI6ImFmOWNlNzg5MWEwZTQ0YzUyMDc5OGE5MDIwZTQyOTVjNmJhOGMwMjE0ZTZmMGM3NGI0ZWM4NGNmMDE3MzFhZjMifQ -->
### `client.compute_risk_radar`

Operation ID: `computeRiskRadar`  
Route: `POST` `/v1/reviews/risk-radar`  

#### Signature

```ruby
def compute_risk_radar(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | 6-axis Risk Radar telemetry | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjb21wdXRlUmlza1JhZGFyIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjcmVhdGVfcmV2aWV3IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImNyZWF0ZVJldmlldyIsInBhdGgiOiIvdjEvcmV2aWV3cyIsInJlc291cmNlIjoicmV2aWV3cyIsInNlY3Rpb25fc2hhMjU2IjoiYzY1MDIzYzEwZmIwYWQ5MzU1N2M4MTI4MTExZjM4OTNjYTA1MzQzZjUxMDE0YWE5MjE1ODQ1NjQ4OTBiZGM3NSIsInNpZ25hdHVyZV9zaGEyNTYiOiI0ZGFlMDdjOTE4YjZkYjJhZTdkMzZkOGQzMjYwMzYzZjgwNGQ5YjZhZDFjZGZmZDhhNmVmYjE0NDA4NmNmMWU1In0 -->
### `client.create_review`

Operation ID: `createReview`  
Route: `POST` `/v1/reviews`  

#### Signature

```ruby
def create_review(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Completed review result with findings, blast radius, and change stack | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVSZXZpZXcifQ -->

## Resource `saas`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJmaW5hbGl6ZV9tZXRlcmluZ19xdW90YSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJmaW5hbGl6ZU1ldGVyaW5nUXVvdGEiLCJwYXRoIjoiL3YxL3NhYXMvbWV0ZXJpbmcvZmluYWxpemUiLCJyZXNvdXJjZSI6InNhYXMiLCJzZWN0aW9uX3NoYTI1NiI6ImJmYjFmMzVmMGUwODE5YTE0YmQzZGFhMjNlNzQxZWU2YTA3MGVkMDkyZWRjMmU0NDhlNTVkNGJlNzc3MWQ1MjYiLCJzaWduYXR1cmVfc2hhMjU2IjoiZTkyMjM5YjM3NDVkNzVjMmVlNDM4NjY5NjUwYmRlMWUwMzI5YzQyMTczNzc5ZWMzYzQxYzA4MWM0NjFkMmZmZCJ9 -->
### `client.finalize_metering_quota`

Operation ID: `finalizeMeteringQuota`  
Route: `POST` `/v1/saas/metering/finalize`  

#### Signature

```ruby
def finalize_metering_quota(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Finalized metering settlement | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJmaW5hbGl6ZU1ldGVyaW5nUXVvdGEifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfc2Fhc19ibHVlcHJpbnQiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRTYWFzQmx1ZXByaW50IiwicGF0aCI6Ii92MS9zYWFzL2JsdWVwcmludCIsInJlc291cmNlIjoic2FhcyIsInNlY3Rpb25fc2hhMjU2IjoiMDk5Nzk4OWIxNGM4MTY4YTIyZTI1NWIxMTViNzgzMDE0OTZhOTgxOTRmNWUyOGNhYTYyOGRmNjM3NzNhYjFlMCIsInNpZ25hdHVyZV9zaGEyNTYiOiJhMmI1MDY4NTllMWM5OTVkYzllNDI1NGVlNWYyOTA5ZTc1NDkwMDJkZTFiNDhlZTUyOWQ1MWYxZTYyNmUzYWE4In0 -->
### `client.get_saas_blueprint`

Operation ID: `getSaasBlueprint`  
Route: `GET` `/v1/saas/blueprint`  

#### Signature

```ruby
def get_saas_blueprint()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Autonomous SaaS blueprint | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRTYWFzQmx1ZXByaW50In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJpc3N1ZV9zdXJmYWNlX2xlYXNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6Imlzc3VlU3VyZmFjZUxlYXNlIiwicGF0aCI6Ii92MS9zYWFzL3N1cmZhY2UtbGVhc2UvaXNzdWUiLCJyZXNvdXJjZSI6InNhYXMiLCJzZWN0aW9uX3NoYTI1NiI6ImRkNjAzYmNjYmQyODVjZWYyYWI0NzdjODc4M2UzYWI5NzQ0N2I4NjhkMjI4MmI0YWU5YTk4ZTFlMGZiYzgwMzMiLCJzaWduYXR1cmVfc2hhMjU2IjoiM2Y0YjFjMzVjNGJiNWNjNTkwZDI1Y2JmNmJjOWEzZTg0MjhiMWI1NjY2MjM0YWQ4ZWU1Njg3ZjhlMjFlMTllNCJ9 -->
### `client.issue_surface_lease`

Operation ID: `issueSurfaceLease`  
Route: `POST` `/v1/saas/surface-lease/issue`  

#### Signature

```ruby
def issue_surface_lease(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Issued surface lease token | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJpc3N1ZVN1cmZhY2VMZWFzZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZXNlcnZlX21ldGVyaW5nX3F1b3RhIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InJlc2VydmVNZXRlcmluZ1F1b3RhIiwicGF0aCI6Ii92MS9zYWFzL21ldGVyaW5nL3Jlc2VydmUiLCJyZXNvdXJjZSI6InNhYXMiLCJzZWN0aW9uX3NoYTI1NiI6IjY4NGNkMGEyZDFmNzgzZWE1YjZjNWY2NWZkYzc0ZmQ2MmI0YzdiNjgwYjdhNmFhMzExZGI0ODIxMDFiM2FlYjAiLCJzaWduYXR1cmVfc2hhMjU2IjoiOTQ2NWYwNWU5MmU4NjY2MmNmYzA3M2IyZThkMzgyMTFkZTc5MGZiZGI2ZDQ4NmYxMjBmMzllOTAzNTU4YTU4OSJ9 -->
### `client.reserve_metering_quota`

Operation ID: `reserveMeteringQuota`  
Route: `POST` `/v1/saas/metering/reserve`  

#### Signature

```ruby
def reserve_metering_quota(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Metering reservation record | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZXNlcnZlTWV0ZXJpbmdRdW90YSJ9 -->

## Resource `sbom`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZW5lcmF0ZV9zYm9tIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImdlbmVyYXRlU2JvbSIsInBhdGgiOiIvdjEvc2JvbSIsInJlc291cmNlIjoic2JvbSIsInNlY3Rpb25fc2hhMjU2IjoiNjIwNjNhNjA3MTM5MzBhYTNmMjk3MzMwOGMyYmYzMDBjNzU2MTc5NGYwNmM3NDU1OGE2MTJmNjEzMzdkYzY4MyIsInNpZ25hdHVyZV9zaGEyNTYiOiJmY2RkNWFiZTEwMThiYzU4MzI5Yjg5MjczOThmYmI4YmU2MDk4NDNmZTQ5NzhiYWI0ZWY4OTYxYTdkOTAxNWUxIn0 -->
### `client.generate_sbom`

Operation ID: `generateSbom`  
Route: `POST` `/v1/sbom`  

#### Signature

```ruby
def generate_sbom(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | CycloneDX 1.5 SBOM JSON | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZW5lcmF0ZVNib20ifQ -->

## Resource `supply_chain`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJhbmFseXplX3N1cHBseV9jaGFpbiIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJhbmFseXplU3VwcGx5Q2hhaW4iLCJwYXRoIjoiL3YxL3N1cHBseS1jaGFpbi9hbmFseXplIiwicmVzb3VyY2UiOiJzdXBwbHlfY2hhaW4iLCJzZWN0aW9uX3NoYTI1NiI6IjRjNDU3YTljZjZkMjIxYzAzOGFiOGViMWYyYzUzY2FhMjRmZGJlNDc2OGVkMmFiN2YwYTFlMTEzZmU4NGQ2MDciLCJzaWduYXR1cmVfc2hhMjU2IjoiODExYzM0NWIyYWQwMmE2NTg2ODNjNmUwN2ZhZDM2MTg2YWIxZGFjOTI5OGNlNmM2YTY5OGU3ODVkMDU5ZmM0NyJ9 -->
### `client.analyze_supply_chain`

Operation ID: `analyzeSupplyChain`  
Route: `POST` `/v1/supply-chain/analyze`  

#### Signature

```ruby
def analyze_supply_chain(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `ReviewRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Supply-chain security audit | none |

#### Canonical required-input example

```json
{
  "body": {
    "files": [
      {
        "filename": "example"
      }
    ]
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJhbmFseXplU3VwcGx5Q2hhaW4ifQ -->

## Resource `tasks`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjcmVhdGVfY29kaW5nX3Rhc2siLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY3JlYXRlQ29kaW5nVGFzayIsInBhdGgiOiIvdjEvdGFza3MiLCJyZXNvdXJjZSI6InRhc2tzIiwic2VjdGlvbl9zaGEyNTYiOiI5NGZlMmFmMDRiYjdjOTgyYWRhMWFkNDFiNjhjZjY0NjM1NDI5NDNhMDJiY2U5YWE0MmY4OWE2NjhhZGRlZDk0Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjQxZTllMjk1ODQ0MTgwNDMwNmEwNDFiNGIyYTljZWFkNGZlOGY1MzBjMjM4YTg5NDdjNDUyZDc5ZDM2ZmY4NDAifQ -->
### `client.create_coding_task`

Operation ID: `createCodingTask`  
Route: `POST` `/v1/tasks`  

#### Signature

```ruby
def create_coding_task(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | Created coding task | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVDb2RpbmdUYXNrIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X2NvZGluZ190YXNrcyIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6Imxpc3RDb2RpbmdUYXNrcyIsInBhdGgiOiIvdjEvdGFza3MiLCJyZXNvdXJjZSI6InRhc2tzIiwic2VjdGlvbl9zaGEyNTYiOiJmZTAzODc5MGFjMjlmYmRhOWUyNjEyY2U1OGM3MjJhY2ZmZjM1NDc3Y2RiMjg0M2FiY2M1ZmFiMzdiMWU0NzlhIiwic2lnbmF0dXJlX3NoYTI1NiI6IjVhNzQzYjM4NmU0OWM1Mjc0YzkyYjNmOGRlMzczMmFmNjk1ODIxNDFiNTU0Y2RiZTlmY2Y4YmQxYWFmMzBiNjQifQ -->
### `client.list_coding_tasks`

Operation ID: `listCodingTasks`  
Route: `GET` `/v1/tasks`  

#### Signature

```ruby
def list_coding_tasks()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Task list | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0Q29kaW5nVGFza3MifQ -->

## Resource `triage`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfdHJpYWdlX3F1ZXVlIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0VHJpYWdlUXVldWUiLCJwYXRoIjoiL3YxL3RyaWFnZSIsInJlc291cmNlIjoidHJpYWdlIiwic2VjdGlvbl9zaGEyNTYiOiIyZTlkNTQ1YWMyNWU3MTczMTM4NGVhNjM1Mzg2ZjljNGQ4MWE1ODcxZmZhMDU1ZTAyMGE5NjA2MDQzYTM4ZjdkIiwic2lnbmF0dXJlX3NoYTI1NiI6IjQ0MzAyZDgzMDhhYzc4YTAwNjZiNGY3ZWU1MmNlNjI1NTg4NWJkYTYzZTFjODg1NmQ3OWM0ZGE2NWRmNTI4ZDUifQ -->
### `client.get_triage_queue`

Operation ID: `getTriageQueue`  
Route: `GET` `/v1/triage`  

#### Signature

```ruby
def get_triage_queue()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Triaged PR queue | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRUcmlhZ2VRdWV1ZSJ9 -->

## Resource `waitlist`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X3dhaXRsaXN0IiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdFdhaXRsaXN0IiwicGF0aCI6Ii92MS93YWl0bGlzdCIsInJlc291cmNlIjoid2FpdGxpc3QiLCJzZWN0aW9uX3NoYTI1NiI6IjI5N2JkYjJjMmZkZWMzMmJhZDUwNDAwYTc3NmFhMTI2YTVhNTUwMmMxYmM5ZjI3YmIzNzlkY2I4ZDM2ZDI5OTciLCJzaWduYXR1cmVfc2hhMjU2IjoiOGVlOTgxNDc5YTU3MjBjMGZlZGU3OTk0YzI3MDk5MzBmNTBhMWQ2NWQ4MGU0OTA4N2U2MTg2MDJjNDc4NWE1NiJ9 -->
### `client.list_waitlist`

Operation ID: `listWaitlist`  
Route: `GET` `/v1/waitlist`  

#### Signature

```ruby
def list_waitlist()
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Waitlist entries | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0V2FpdGxpc3QifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZWdpc3Rlcl93YWl0bGlzdCIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJyZWdpc3RlcldhaXRsaXN0IiwicGF0aCI6Ii92MS93YWl0bGlzdCIsInJlc291cmNlIjoid2FpdGxpc3QiLCJzZWN0aW9uX3NoYTI1NiI6IjFlYWQ1N2U5ZDJhNzQ0NmI5ZTQzNmU1YTE0NmU3ODY1MWIzNWE1MzIzNmY1NGU5MzdlN2Q5ZGI5ZTUxMDVkYjUiLCJzaWduYXR1cmVfc2hhMjU2IjoiZTc5NmNjYzdiYzM5MzI2NDY1NTllMzA3NDMxMzNhZjY2NGMwNDA2Yzk2YTViNDcwMDBkMjFjNTkzZGVkZTU1NyJ9 -->
### `client.register_waitlist`

Operation ID: `registerWaitlist`  
Route: `POST` `/v1/waitlist`  

#### Signature

```ruby
def register_waitlist(body: nil)
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `WaitlistRequest` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | Waitlist entry created | none |

#### Canonical required-input example

```json
{
  "body": {
    "email": "example-c65f@example.test"
  },
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZWdpc3RlcldhaXRsaXN0In0 -->

