# Practical 01 — Windows Failed Authentication

## Objective
Validate detection of failed Windows authentication attempts through Wazuh.

## Telemetry
Windows Security Event ID 4625.

## Wazuh Detection
Rule 60122 — Windows authentication failure.

## Validation
A controlled failed authentication attempt was generated on the Windows endpoint and the corresponding event was received and analyzed by Wazuh.

## SOC Relevance
Repeated authentication failures can indicate password guessing or brute-force activity and require further investigation when correlated with additional events.
