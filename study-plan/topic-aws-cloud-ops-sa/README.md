# AWS Cloud Ops & Solutions Architect SME — Study Plan

A structured, hands-on study plan covering **AWS Certified CloudOps Engineer - Associate (SOA-C03)** and **AWS Certified Solutions Architect - Professional (SAP-C02)** exam domains. Lessons progress from foundational operations to advanced architectural design, culminating in a real-world capstone.

## Companion Track (Integrated)

For hands-on Infrastructure as Code and GitOps practice alongside this AWS path, use:

- [Infrastructure as Code Study Plan (Terraform + Docker + Kubernetes + Argo CD)](../topic-infrastructure-as-code-terraform-docker-kubernetes-argo-cd/README.md)

Suggested pairing:
- Complete AWS Phases 1-2, then IaC Phase 1
- Continue AWS Phases 3-4, then IaC Phase 2
- Finish AWS Phases 5-9, then IaC Phase 3 + IaC capstone

---

## Prerequisites

### Tools to Install
- [ ] [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) — `aws --version`
- [ ] [Python 3.10+](https://www.python.org/downloads/) — `python --version`
- [ ] [Jupyter Lab / Notebook](https://jupyter.org/install) — `pip install jupyterlab`
- [ ] [boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html) — `pip install boto3`
- [ ] [cfn-lint](https://github.com/aws-cloudformation/cfn-lint) — `pip install cfn-lint` (optional but recommended)

### AWS Account Setup
- [ ] An AWS account (Free Tier is sufficient for most lessons)
- [ ] An IAM user with programmatic access and `AdministratorAccess` (for learning only; scope down in prod)
- [ ] AWS credentials configured: `aws configure`

### Prior Knowledge Assumed
- Basic Linux/terminal comfort
- Basic networking concepts (IP, DNS, TCP/UDP, firewalls)
- Familiarity with YAML/JSON
- No prior AWS expertise required for Phase 1–2; Phases 7–9 assume Phase 1–6 complete

---

## Recommended Resources

### 📋 Official Exam Guides
| Resource | URL |
|----------|-----|
| SOA-C03 Exam Guide | https://docs.aws.amazon.com/aws-certification/latest/sysops-administrator-associate-03/ |
| SOA-C03 In-Scope Services | https://docs.aws.amazon.com/aws-certification/latest/sysops-administrator-associate-03/soa-03-in-scope-services.html |
| SAP-C02 Exam Guide | https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-professional-02/solutions-architect-professional-02.html |
| SAP-C02 In-Scope Services | https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-professional-02/sap-02-in-scope-services.html |
| All AWS Certification Exam Guides | https://docs.aws.amazon.com/aws-certification/latest/examguides/aws-certification-exam-guides.html |

### 📚 AWS Official Documentation
| Resource | URL |
|----------|-----|
| AWS Documentation (all services) | https://docs.aws.amazon.com/ |
| AWS Well-Architected Framework | https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html |
| AWS Architecture Center | https://aws.amazon.com/architecture/ |
| AWS Whitepapers | https://aws.amazon.com/whitepapers/ |
| AWS Prescriptive Guidance | https://docs.aws.amazon.com/prescriptive-guidance/latest/patterns/welcome.html |
| AWS CLI Reference | https://docs.aws.amazon.com/cli/latest/reference/ |
| boto3 Documentation | https://boto3.amazonaws.com/v1/documentation/api/latest/index.html |

### 🎓 Training Platforms
| Resource | URL |
|----------|-----|
| AWS Skill Builder (Exam Prep + Free Labs) | https://skillbuilder.aws/#exam-prep |
| Stephane Maarek — SOA / SAA / SAP (Udemy) | https://www.udemy.com/user/stephane-maarek/ |
| Adrian Cantrill — SA-Pro (deepest coverage) | https://learn.cantrill.io/ |
| Jon Bonso / Tutorials Dojo Practice Exams | https://portal.tutorialsdojo.com/ |
| A Cloud Guru / Pluralsight | https://acloudguru.com/ |

### 📝 Cheat Sheets & Quick Reference
| Resource | URL |
|----------|-----|
| Tutorials Dojo AWS Cheat Sheets | https://tutorialsdojo.com/aws-cheat-sheets/ |
| AWS Services Summary (Tutorials Dojo) | https://tutorialsdojo.com/aws-cheat-sheets/#aws-services-summary |
| AWS IAM Policy Reference | https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements.html |
| CloudFormation Resource Reference | https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html |
| EC2 Instance Types Comparison | https://instances.vantage.sh/ |
| AWS Pricing Calculator | https://calculator.aws/ |

### 🛠️ Key Service Docs (Bookmarks by Phase)
| Phase | Service | URL |
|-------|---------|-----|
| 2 | CloudWatch | https://docs.aws.amazon.com/cloudwatch/latest/monitoring/ |
| 2 | CloudWatch Logs Insights Syntax | https://docs.aws.amazon.com/cloudwatch/latest/logs/CWL_QuerySyntax.html |
| 2 | AWS Systems Manager | https://docs.aws.amazon.com/systems-manager/latest/userguide/ |
| 2 | CloudTrail | https://docs.aws.amazon.com/cloudtrail/latest/userguide/ |
| 3 | ELB User Guide | https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/ |
| 3 | Auto Scaling | https://docs.aws.amazon.com/autoscaling/ec2/userguide/ |
| 3 | RDS Multi-AZ | https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html |
| 4 | CloudFormation | https://docs.aws.amazon.com/cloudformation/latest/userguide/ |
| 4 | AWS CDK v2 | https://docs.aws.amazon.com/cdk/v2/guide/ |
| 4 | CodeDeploy | https://docs.aws.amazon.com/codedeploy/latest/userguide/ |
| 5 | IAM Policy Reference | https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements.html |
| 5 | AWS KMS | https://docs.aws.amazon.com/kms/latest/developerguide/ |
| 5 | Secrets Manager | https://docs.aws.amazon.com/secretsmanager/latest/userguide/ |
| 5 | AWS Config | https://docs.aws.amazon.com/config/latest/developerguide/ |
| 6 | VPC User Guide | https://docs.aws.amazon.com/vpc/latest/userguide/ |
| 6 | Transit Gateway | https://docs.aws.amazon.com/vpc/latest/tgw/ |
| 6 | Route 53 | https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/ |
| 6 | CloudFront | https://docs.aws.amazon.com/cloudfront/latest/APIReference/ |
| 7 | AWS Organizations | https://docs.aws.amazon.com/organizations/latest/userguide/ |
| 7 | Control Tower | https://docs.aws.amazon.com/controltower/latest/userguide/ |
| 7 | Direct Connect | https://docs.aws.amazon.com/directconnect/latest/UserGuide/ |
| 8 | Lambda | https://docs.aws.amazon.com/lambda/latest/dg/ |
| 8 | ECS | https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ |
| 8 | DynamoDB | https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/ |
| 9 | AWS DMS | https://docs.aws.amazon.com/dms/latest/userguide/ |
| 9 | AWS MGN | https://docs.aws.amazon.com/mgn/latest/ug/ |
| 9 | AWS Migration Hub | https://docs.aws.amazon.com/migrationhub/latest/ug/ |

### 🆓 Free Tier & Account
| Resource | URL |
|----------|-----|
| AWS Free Tier | https://aws.amazon.com/free/ |
| AWS Free Tier Usage Alerts | https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/tracking-free-tier-usage.html |
| AWS re:Post (community Q&A) | https://repost.aws/ |
| AWS Events & re:Invent talks | https://www.youtube.com/@AWSEventsChannel |

---

## Study Plan Overview

| Phase | Title | Exam Domain | Lessons | Est. Time |
|-------|-------|-------------|---------|-----------|
| 1 | AWS Foundations & Well-Architected Framework | Both | 4 | 4–6 hrs |
| 2 | Monitoring, Logging & Observability | SOA-C03 Domain 1 (22%) | 5 | 5–7 hrs |
| 3 | Reliability & Business Continuity | SOA-C03 Domain 2 (22%) | 4 | 4–6 hrs |
| 4 | Deployment, Provisioning & Automation | SOA-C03 Domain 3 (22%) | 5 | 6–8 hrs |
| 5 | Security & Compliance | SOA-C03 Domain 4 (16%) | 3 | 4–5 hrs |
| 6 | Networking & Content Delivery | SOA-C03 Domain 5 (18%) | 4 | 5–6 hrs |
| 7 | Organizational Complexity & Multi-Account | SAP-C02 Domain 1 (26%) | 4 | 5–7 hrs |
| 8 | New Solutions — HA, Performance & Serverless | SAP-C02 Domain 2 (29%) | 4 | 5–7 hrs |
| 9 | Migration, Modernization & Continuous Improvement | SAP-C02 Domains 3 & 4 | 4 | 5–7 hrs |
| — | Capstone | Both Certs | 1 | 8–12 hrs |

**Total: 37 lessons + 1 capstone | Estimated 51–71 hours**

---

## Lessons

### Phase 1 — AWS Foundations & Well-Architected Framework
| # | Notebook | Topic |
|---|----------|-------|
| 1.1 | [lesson-1.1-aws-global-iam.ipynb](phase-1-foundations/lesson-1.1-aws-global-iam.ipynb) | AWS Global Infrastructure & IAM Fundamentals |
| 1.2 | [lesson-1.2-well-architected.ipynb](phase-1-foundations/lesson-1.2-well-architected.ipynb) | AWS Well-Architected Framework (6 Pillars) |
| 1.3 | [lesson-1.3-aws-cli-boto3.ipynb](phase-1-foundations/lesson-1.3-aws-cli-boto3.ipynb) | AWS CLI & boto3 — Automation Fundamentals |
| 1.4 | [lesson-1.4-cloudformation-basics.ipynb](phase-1-foundations/lesson-1.4-cloudformation-basics.ipynb) | CloudFormation Basics — Infrastructure as Code |

### Phase 2 — Monitoring, Logging & Observability
| # | Notebook | Topic |
|---|----------|-------|
| 2.1 | [lesson-2.1-cloudwatch-metrics-alarms.ipynb](phase-2-monitoring/lesson-2.1-cloudwatch-metrics-alarms.ipynb) | CloudWatch Metrics, Alarms & Dashboards |
| 2.2 | [lesson-2.2-cloudwatch-logs.ipynb](phase-2-monitoring/lesson-2.2-cloudwatch-logs.ipynb) | CloudWatch Logs, Log Insights & CloudWatch Agent |
| 2.3 | [lesson-2.3-cloudtrail-eventbridge.ipynb](phase-2-monitoring/lesson-2.3-cloudtrail-eventbridge.ipynb) | CloudTrail, EventBridge & SNS Notifications |
| 2.4 | [lesson-2.4-systems-manager.ipynb](phase-2-monitoring/lesson-2.4-systems-manager.ipynb) | Systems Manager Automation & Runbooks |
| 2.5 | [lesson-2.5-performance-optimization.ipynb](phase-2-monitoring/lesson-2.5-performance-optimization.ipynb) | Performance Optimization — EC2, EBS, RDS, S3 |

### Phase 3 — Reliability & Business Continuity
| # | Notebook | Topic |
|---|----------|-------|
| 3.1 | [lesson-3.1-auto-scaling-elb.ipynb](phase-3-reliability/lesson-3.1-auto-scaling-elb.ipynb) | Auto Scaling Groups & Elastic Load Balancing |
| 3.2 | [lesson-3.2-multi-az-region.ipynb](phase-3-reliability/lesson-3.2-multi-az-region.ipynb) | Multi-AZ & Multi-Region Architectures |
| 3.3 | [lesson-3.3-disaster-recovery.ipynb](phase-3-reliability/lesson-3.3-disaster-recovery.ipynb) | Disaster Recovery Patterns (RTO/RPO) |
| 3.4 | [lesson-3.4-backup-restore.ipynb](phase-3-reliability/lesson-3.4-backup-restore.ipynb) | AWS Backup, Snapshots & Data Versioning |

### Phase 4 — Deployment, Provisioning & Automation
| # | Notebook | Topic |
|---|----------|-------|
| 4.1 | [lesson-4.1-amis-image-builder.ipynb](phase-4-deployment/lesson-4.1-amis-image-builder.ipynb) | EC2 AMIs, Launch Templates & EC2 Image Builder |
| 4.2 | [lesson-4.2-cloudformation-advanced.ipynb](phase-4-deployment/lesson-4.2-cloudformation-advanced.ipynb) | CloudFormation Advanced — StackSets, Nested Stacks, CDK |
| 4.3 | [lesson-4.3-deployment-strategies.ipynb](phase-4-deployment/lesson-4.3-deployment-strategies.ipynb) | Deployment Strategies — Blue/Green, Rolling, Canary |
| 4.4 | [lesson-4.4-ssm-parameter-store.ipynb](phase-4-deployment/lesson-4.4-ssm-parameter-store.ipynb) | SSM OpsCenter, Parameter Store & Patch Manager |
| 4.5 | [lesson-4.5-event-driven-automation.ipynb](phase-4-deployment/lesson-4.5-event-driven-automation.ipynb) | Event-Driven Automation — Lambda, S3 Events, EventBridge |

### Phase 5 — Security & Compliance
| # | Notebook | Topic |
|---|----------|-------|
| 5.1 | [lesson-5.1-iam-advanced.ipynb](phase-5-security/lesson-5.1-iam-advanced.ipynb) | IAM Deep Dive — Roles, SCPs, Identity Center, Organizations |
| 5.2 | [lesson-5.2-encryption-secrets.ipynb](phase-5-security/lesson-5.2-encryption-secrets.ipynb) | Encryption at Rest & In Transit — KMS, ACM, Secrets Manager |
| 5.3 | [lesson-5.3-compliance-tools.ipynb](phase-5-security/lesson-5.3-compliance-tools.ipynb) | Compliance — AWS Config, Security Hub, GuardDuty, Inspector |

### Phase 6 — Networking & Content Delivery
| # | Notebook | Topic |
|---|----------|-------|
| 6.1 | [lesson-6.1-vpc-fundamentals.ipynb](phase-6-networking/lesson-6.1-vpc-fundamentals.ipynb) | VPC Deep Dive — Subnets, Route Tables, NAT, SGs, NACLs |
| 6.2 | [lesson-6.2-vpc-connectivity.ipynb](phase-6-networking/lesson-6.2-vpc-connectivity.ipynb) | VPC Connectivity — Peering, PrivateLink, Endpoints, Transit GW |
| 6.3 | [lesson-6.3-route53-dns.ipynb](phase-6-networking/lesson-6.3-route53-dns.ipynb) | Route 53 — Routing Policies, Health Checks, DNS Firewall |
| 6.4 | [lesson-6.4-cloudfront-waf.ipynb](phase-6-networking/lesson-6.4-cloudfront-waf.ipynb) | CloudFront, WAF, Shield & Global Accelerator |

### Phase 7 — Organizational Complexity & Multi-Account (SAP-C02 Domain 1)
| # | Notebook | Topic |
|---|----------|-------|
| 7.1 | [lesson-7.1-multi-account.ipynb](phase-7-org-complexity/lesson-7.1-multi-account.ipynb) | Multi-Account Strategy — Organizations, Control Tower, RAM |
| 7.2 | [lesson-7.2-hybrid-networking.ipynb](phase-7-org-complexity/lesson-7.2-hybrid-networking.ipynb) | Advanced Networking — Direct Connect, VPN, Hybrid Architectures |
| 7.3 | [lesson-7.3-advanced-security-arch.ipynb](phase-7-org-complexity/lesson-7.3-advanced-security-arch.ipynb) | Advanced Security Architecture — Cross-Account, SCP Design |
| 7.4 | [lesson-7.4-cost-optimization.ipynb](phase-7-org-complexity/lesson-7.4-cost-optimization.ipynb) | Cost Optimization — Cost Explorer, Savings Plans, Tagging |

### Phase 8 — New Solutions: HA, Performance & Serverless (SAP-C02 Domain 2)
| # | Notebook | Topic |
|---|----------|-------|
| 8.1 | [lesson-8.1-ha-fault-tolerant.ipynb](phase-8-new-solutions/lesson-8.1-ha-fault-tolerant.ipynb) | Designing HA & Fault-Tolerant Architectures |
| 8.2 | [lesson-8.2-performance-databases.ipynb](phase-8-new-solutions/lesson-8.2-performance-databases.ipynb) | Performance Architecture — Caching, Purpose-Built Databases |
| 8.3 | [lesson-8.3-serverless-containers.ipynb](phase-8-new-solutions/lesson-8.3-serverless-containers.ipynb) | Serverless & Containers — Lambda, ECS, EKS, Fargate |
| 8.4 | [lesson-8.4-application-integration.ipynb](phase-8-new-solutions/lesson-8.4-application-integration.ipynb) | Application Integration — SQS, SNS, Step Functions, EventBridge |

### Phase 9 — Migration, Modernization & Continuous Improvement (SAP-C02 Domains 3 & 4)
| # | Notebook | Topic |
|---|----------|-------|
| 9.1 | [lesson-9.1-migration-assessment.ipynb](phase-9-migration/lesson-9.1-migration-assessment.ipynb) | Migration Assessment — 7Rs Framework & Migration Hub |
| 9.2 | [lesson-9.2-database-migration.ipynb](phase-9-migration/lesson-9.2-database-migration.ipynb) | Database Migration — AWS DMS & Schema Conversion Tool |
| 9.3 | [lesson-9.3-application-migration.ipynb](phase-9-migration/lesson-9.3-application-migration.ipynb) | Application Migration — AWS MGN, DataSync, Snow Family |
| 9.4 | [lesson-9.4-modernization.ipynb](phase-9-migration/lesson-9.4-modernization.ipynb) | Modernization — Serverless, Containers & Purpose-Built DBs |

### Capstone
| Notebook | Description |
|----------|-------------|
| [capstone/capstone-project.ipynb](capstone/capstone-project.ipynb) | Deploy a production-grade multi-account AWS environment with 3-tier app, full observability, DR, and CI/CD |

---

## Capstone Overview

**Scenario:** You are the lead Solutions Architect & CloudOps Engineer for a fintech startup. Design and operationalize a production-grade AWS environment that includes:

- A **multi-account structure** (management, dev, staging, prod) with AWS Organizations and Control Tower
- A **3-tier web application** (ALB → ECS Fargate → Aurora RDS) deployed via CloudFormation
- **Full observability** stack: CloudWatch dashboards, alarms, log groups, X-Ray tracing
- **Security controls**: KMS encryption, Secrets Manager, GuardDuty, Config rules, WAF
- **Disaster recovery** plan with RTO ≤ 4 hours, RPO ≤ 1 hour (pilot light pattern)
- **CI/CD pipeline** with blue/green deployment using CodePipeline + CodeDeploy
- **Cost governance**: budget alarms, Savings Plans analysis, tagging strategy

---

## How to Use These Notebooks

1. Install Jupyter: `pip install jupyterlab`
2. Launch: `jupyter lab` (from within the `study-plan/topic-aws-cloud-ops-sa/` directory)
3. Open lessons in phase order — each builds on the previous
4. Run cells top-to-bottom — do NOT skip cells
5. Complete `# TODO:` exercises before moving to the next lesson
6. AWS CLI commands require valid credentials: `aws configure`

> **Cost awareness:** Most exercises use free-tier-eligible services. Commands that create billable resources (EC2, RDS, etc.) include a **cleanup cell** at the bottom of each notebook. Always run cleanup cells after practicing.
