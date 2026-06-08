---
category: runbook
title: API Gateway runbook
description: On-call runbook for API Gateway.
related_entities:
  - api-gateway
related_teams:
  - platform
---

# API Gateway runbook

On-call guide for `api-gateway` (Platform, tier critical).

## Alerts

- **api-gateway-high-error-rate** — 5xx over 2% for 5m. Check upstream dependencies.
- **api-gateway-latency** — p99 over SLO. Check resource saturation.

## Common issues

- **Pod OOMKilled** — check memory limits and recent traffic spikes.
- **Crashloop** — check the last deploy and roll back if needed.

## Escalation

Page the Platform on-call rotation.

