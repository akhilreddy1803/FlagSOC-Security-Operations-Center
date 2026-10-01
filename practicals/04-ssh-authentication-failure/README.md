# Practical 04 — SSH Authentication Failure

## Objective
Validate monitoring of failed SSH authentication attempts on a Linux endpoint.

## Telemetry
Linux SSH/PAM authentication failure events.

## Wazuh Detection
Rule 5503 — SSH authentication failure.

## Validation
Controlled SSH authentication failures were generated and the corresponding events were received by Wazuh.

## SOC Relevance
Repeated SSH authentication failures can indicate password guessing or brute-force activity and should be investigated in context.
