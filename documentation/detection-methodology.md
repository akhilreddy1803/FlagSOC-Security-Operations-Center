# FlagSOC Detection Engineering Methodology

## Purpose

This document describes the approach used to create and validate security detections in the FlagSOC SOC lab.

## Detection Process

1. Identify the security activity to monitor.
2. Verify available telemetry sources.
3. Analyze the generated security events.
4. Create or tune Wazuh detection logic.
5. Validate alerts using controlled testing.
6. Document the detection.

## Telemetry Sources

- Windows Security Events
- Sysmon Events
- Linux SSH Authentication Logs
- Wazuh Agent Telemetry

## Custom Detections

The project includes:

- FLAGSOC-DET-001: Windows Local Brute Force
- FLAGSOC-DET-002: Successful Login After Brute Force
- FLAGSOC-DET-003: SSH Brute Force

## Validation

Each detection was tested in an authorized lab environment by generating controlled events and confirming alert generation in Wazuh.

