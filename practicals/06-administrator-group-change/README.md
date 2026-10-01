# Practical 06 — Administrator Group Change

## Objective
Detect changes to the local Windows Administrators security group.

## Windows Event
Event ID 4732/4733.

## Wazuh Detection
Rule 60154 — Administrator/security group membership change.

## Telemetry Prerequisite
Windows Security Group Management auditing must be enabled for the required security events to be generated.

## Validation
A controlled user was added to the local Administrators group. The resulting Windows security event was received by Wazuh and generated the expected detection.

## SOC Relevance
Unauthorized changes to privileged groups can provide elevated access and should be investigated.
