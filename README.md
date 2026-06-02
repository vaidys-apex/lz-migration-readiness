# Contoso Financial Services — Landing Zone Current State

This repository contains CloudFormation templates representing the **current state** of Contoso Financial Services' AWS Landing Zone infrastructure, as assessed on June 2, 2026.

**Assessment Scope:** 347 applications, 1,214 servers, 189 databases
**Overall Maturity:** 3.0/5 (Defined)

## Structure

```
infrastructure/
├── network-connectivity/      # Transit Gateway hub-and-spoke, Direct Connect, VPCs
├── network-security/          # SCPs, Security Groups, NACLs
├── workload-isolation/        # Multi-account strategy, environment segmentation
└── automation/                # Control Tower baseline, CfCT automation
```

## What This Represents

These templates reflect the **strengths** identified in the LZ Readiness Assessment — the capabilities that are already implemented and operational. The **gaps** identified in the assessment (IPAM, VPC Flow Logs retention, capacity planning, template versioning) are intentionally absent from this codebase, representing work that remains to be done.

## Infrastructure Pillar (4/5 — Managed)

### Implemented (in this repo)
- Multi-Account Foundation with Control Tower
- Hub-and-spoke networking with Transit Gateway
- Dual 10Gbps Direct Connect hybrid connectivity
- 3-tier VPC design (web/app/data)
- Centralized egress with NACLs and Security Groups
- Workload isolation via dedicated VPCs per environment

### Not Implemented (gaps — not in this repo)
- Centralized IPAM solution
- VPC Flow Logs with defined retention
- Network capacity planning / Direct Connect monitoring
- CfCT template versioning and rollback
