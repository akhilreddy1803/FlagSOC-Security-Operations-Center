# Practical 05 — SSH Brute Force

## Objective
Detect repeated SSH authentication failures.

## Detection
FLAGSOC-DET-003 — Wazuh Rule 100102.

## Logic
Three matching SSH authentication failure events within 60 seconds.

## Base Detection
Wazuh Rule 5503.

## MITRE ATT&CK
T1110.001 — Password Guessing.

## Validation
The custom SSH brute-force detection was tested using controlled authentication failures and validated through Wazuh.
