# Project 06 — AWS Cost Monitoring & Budget Alerts

## Project Overview

This project demonstrates the design and implementation of an AWS cost-monitoring and alerting solution using AWS Budgets, Amazon SNS, and Amazon CloudWatch.

The solution provides visibility into estimated AWS charges, establishes spending thresholds, delivers email notifications through Amazon SNS, and presents billing metrics through a centralized CloudWatch dashboard.

## Objective

The objectives of this project were to:

- Monitor estimated AWS charges
- Establish 50%, 80%, and 100% budget thresholds
- Send budget notifications through Amazon SNS
- Confirm an email-based SNS subscription
- Visualize billing metrics through Amazon CloudWatch
- Build a centralized cost-monitoring dashboard
- Demonstrate responsible AWS cost management

## Architecture

![Project 06 AWS Cost Monitoring Architecture](./Project06_AWS_Cost_Monitoring_Architecture.png)

### Architecture Flow

AWS Budget  
→ 50% / 80% / 100% thresholds  
→ Amazon SNS  
→ Confirmed email subscription

AWS Billing / Estimated Charges  
→ CloudWatch Billing Alerts  
→ EstimatedCharges metric  
→ CloudWatch Cost Monitoring Dashboard

## AWS Services Used

| AWS Service | Purpose |
|---|---|
| AWS Budgets | Created Project06-AWS-Cost-Budget with 50%, 80%, and 100% thresholds |
| Amazon SNS | Created Project06-Budget-Alerts for budget notification delivery |
| Amazon CloudWatch | Enabled billing alerts, accessed billing metrics, and created the monitoring dashboard |
| AWS Billing and Cost Management | Configured the project budget and cost-alert preferences |

## Implementation

### 1. AWS Budget

Created:

`Project06-AWS-Cost-Budget`

Configured spending thresholds at:

- 50%
- 80%
- 100%

No automated budget actions were configured.

### 2. Amazon SNS

Created the SNS topic:

`Project06-Budget-Alerts`

Configured an email subscription and successfully confirmed the subscription.

### 3. CloudWatch Billing Alerts

Enabled CloudWatch billing alerts and accessed AWS Billing metrics in the US East (N. Virginia) region.

Primary metric:

`EstimatedCharges`

### 4. CloudWatch Dashboard

Created:

`Project06-AWS-Cost-Monitoring`

The dashboard contains:

- EstimatedCharges for overall estimated AWS cost visibility
- Cost by AWS Service for service-level billing visibility

The dashboard was organized for clear cost monitoring and operational visibility.

## Cost and Security Considerations

- Avoided unnecessary compute, database, or networking resources.
- Used AWS-native billing and monitoring capabilities.
- Configured threshold-based notifications for early cost awareness.
- Redacted personal email addresses from public portfolio screenshots.
- Did not include passwords, access keys, secret keys, or other authentication credentials in the repository.
- Redacted AWS account identifiers from applicable public screenshots where practical.

## Project Evidence

Implementation screenshots are available in the:

[Project 06 Screenshots](./screenshots/)

The screenshots document the major configuration and verification stages, including:

- Budget creation
- Budget thresholds
- SNS topic creation
- Email subscription confirmation
- SNS notification configuration
- CloudWatch billing configuration
- EstimatedCharges metric
- CloudWatch dashboard
- Cost by AWS Service widget
- Final dashboard configuration

## Project Summary

[Download the 1-page Project 06 Summary](./Project06_AWS_Cost_Monitoring_Summary_REVISED.pdf)

## Skills Demonstrated

- AWS Cost Governance
- AWS Budgets
- Amazon SNS
- Amazon CloudWatch
- CloudWatch Billing Metrics
- Cost Monitoring
- Threshold-Based Alerting
- CloudWatch Dashboard Configuration
- AWS Console Troubleshooting
- Operational Documentation

## Project Outcome

Successfully implemented a low-overhead AWS cost-monitoring solution combining budget thresholds, SNS email notification, CloudWatch billing metrics, and centralized dashboard visibility.

The project demonstrates practical AWS cost-governance principles and responsible cloud resource management.

## Key Takeaway

AWS-native services can be combined to create a practical cost-monitoring and alerting architecture without deploying unnecessary infrastructure.
