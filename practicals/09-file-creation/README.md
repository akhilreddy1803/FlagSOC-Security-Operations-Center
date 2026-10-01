# Practical 09 — File Creation Detection

## Objective
Validate Sysmon file creation telemetry and Wazuh alerting.

## Telemetry
Sysmon Event ID 11 — File Create.

## Controlled Test
A controlled executable file was created in C:\Users\Public using PowerShell.

## Wazuh Detection
Rule 92207 — File creation detection observed for the controlled FlagSOC-Test.exe test.

## Validation
Sysmon recorded the file creation event including the creating process, target filename, and user. Wazuh received the event and generated the corresponding alert.

## SOC Relevance
File creation telemetry can help analysts investigate suspicious payload delivery, executable creation, and other endpoint activity.
