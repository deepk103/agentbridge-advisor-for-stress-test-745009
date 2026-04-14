# Architecture Documentation

## Overview
This RAG implements Advisor for Stress Test for Banking & Finance use cases.

## Components
1. **Transfer Intake**: Collect, validate and normalize statements from Case Management; attach a runId and timestamp for traceability.
2. **Retrieve**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Ground**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Risk Scoring**: Risk Scoring across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Portfolio Check**: Portfolio Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Sanctions Screening**: Sanctions Screening across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Limit Control**: Limit Control across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Underwriting**: Underwriting across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
9. **Break Resolution**: Break Resolution across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
10. **Case Closure**: Assemble final payload with status, artifacts, KPIs and audit trail; store to SWIFT Gateway; return response JSON for the client.

## Data Flow
- Input: Transfer Intake
- Processing: 10 sequential steps
- Output: Case Closure
