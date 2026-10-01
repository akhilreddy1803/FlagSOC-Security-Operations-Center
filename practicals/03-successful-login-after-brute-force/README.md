# Practical 03 — Successful Login After Brute Force

## Objective
Detect a successful Windows login occurring after a previously detected brute-force pattern.

## Detection
FLAGSOC-DET-002 — Wazuh Rule 100101.

## Logic
A successful login is correlated with the previous FLAGSOC-DET-001 brute-force detection for the same username within the defined time window.

## Base Detection
Wazuh Rule 60118 — Successful Windows authentication.

## MITRE ATT&CK
T1110 — Brute Force.
T1078 — Valid Accounts.

## Validation
The correlation rule was tested using controlled authentication activity and validated through Wazuh alerts.
