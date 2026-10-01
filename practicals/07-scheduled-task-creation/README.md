# Practical 07 — Scheduled Task Creation

## Objective
Validate monitoring of Windows scheduled task creation.

## Windows Event
Event ID 4698.

## Wazuh Detection
Rule 60228 — A scheduled task was created.

## MITRE ATT&CK
T1053 — Scheduled Task/Job.

## Validation
A new controlled scheduled task named FlagSOC-NewTestTask was created. Windows generated Event 4698 and Wazuh detected it using rule 60228.
