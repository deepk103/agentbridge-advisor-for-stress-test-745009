# API Documentation

## Endpoints
### Transfer Intake
- **Description**: Collect, validate and normalize statements from Case Management; attach a runId and timestamp for traceability.
- **Type**: Processing

### Retrieve
- **Description**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Ground
- **Description**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Risk Scoring
- **Description**: Risk Scoring across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Portfolio Check
- **Description**: Portfolio Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Sanctions Screening
- **Description**: Sanctions Screening across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Limit Control
- **Description**: Limit Control across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Underwriting
- **Description**: Underwriting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Break Resolution
- **Description**: Break Resolution across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Case Closure
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to SWIFT Gateway; return response JSON for the client.
- **Type**: Processing
