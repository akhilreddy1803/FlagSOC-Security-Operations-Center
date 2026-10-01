# Practical 02 — Windows Brute Force

## Objective
Detect repeated failed Windows authentication attempts against the same account.

## Detection
FLAGSOC-DET-001 — Wazuh Rule 100100.

## Logic
Five matching Windows authentication failures within 60 seconds against the same username.

## Base Detection
Wazuh Rule 60122 — Windows failed authentication.

## MITRE ATT&CK
T1110 — Brute Force.

## Validation
The detection was tested using controlled authentication failures and the custom Wazuh rule generated an alert.
