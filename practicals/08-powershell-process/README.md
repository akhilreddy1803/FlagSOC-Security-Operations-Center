# Practical 08 — PowerShell Process Detection

## Objective
Validate endpoint telemetry for PowerShell process creation.

## Telemetry
Sysmon Event ID 1 — Process Creation.

## Wazuh Detection
Rule 92027 — Powershell process spawned powershell instance.

## Validation
A controlled PowerShell process was launched on the Windows endpoint and the corresponding Sysmon telemetry was received by Wazuh.

## SOC Relevance
PowerShell is a legitimate administrative tool but can also be used during attacks, making process telemetry useful for investigation and detection.
