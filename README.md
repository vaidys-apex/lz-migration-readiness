# Contoso Financial Services — Landing Zone Current State

This repository contains CloudFormation templates representing the **current state** of Contoso Financial Services' AWS Landing Zone infrastructure, as assessed on June 2, 2026.

**Overall Maturity:** 3.0/5 (Defined)

## Structure

```
infrastructure/
├── network-connectivity/      # Transit Gateway hub-and-spoke, Direct Connect, VPCs
├── network-security/          # SCPs, Security Groups, NACLs
├── workload-isolation/        # Multi-account strategy, environment segmentation
└── automation/                # Control Tower baseline, CfCT automation
```

