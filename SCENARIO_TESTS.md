# SCENARIO_TESTS.md — Bynder Connector

## Scenario Tests Execution & Evidence
1. **Connection Lifecycle**:
   - `connect_bynder`: Registers OAuth token, saves encrypted config.
   - `list_connections`: Reads active connection, masks token.
   - `disconnect_bynder`: Idempotent removal of credentials.
2. **Asset Retrieval**:
   - `list_assets`: Queries Bynder library with pagination/filters.
   - `get_asset`: Fetches asset metadata and renditions.
3. **Collections & Taxonomy**:
   - `list_collections`: Reads DAM albums and folders.
4. **Health Audit**:
   - `audit_dam_health`: Summarizes asset formats and availability.
5. **PST Part D Verification**:
   - D1: Idempotency checked.
   - D2: Masked secrets only.
   - D3: Regression clean.
