# Workflow Runbook

## Pre-run
- Confirm n8n credentials are valid.
- Confirm external API quotas are healthy.
- Confirm destination CMS/channel is reachable.

## Run
- Execute workflow manually once after any structural change.
- Validate output formatting before enabling scheduled runs.

## Post-run
- Review execution logs for failed nodes.
- Retry idempotent failures only.

## Rollback
- Revert to prior exported workflow version.
- Disable schedule if repeated failures occur.
