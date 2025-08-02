# Study Notes 7/31

## Domain: [AWS Security / Offensive Security / Kubernetes Security]

### Topic: [AWS Exam Overview]

### Primary Resources
- [AWS Official Exam Guide](https://d1.awsstatic.com/onedam/marketing-channels/website/aws/en_US/certification/approved/pdfs/docs-security-spec/AWS-Certified-Security-Specialty_Exam-Guide.pdf)
- [Tutorials Dojo - AWS SCS-C02 Study Guide](./Tutorials-Dojo-Study-Guide-AWS-Certified-Security-Specialty-2024-04-18-zrgfrm.pdf)

### In addition to the 6 domains of the exam the exam also validates:
- An understanding of specialized data classifications and AWS data protection mechanisms
- An understanding of data-encryption methods and AWS mechanisms to implement them
- An understanding of secure internet protocols and AWS mechanisms to implement them
- A working knowledge of AWS security services and features of services to provide a secure production environment
- Competency from 2 or more years of production deployment experience in using AWS security services and features
- The ability to make tradeoff decisions regarding cost, security, and deployment complexity to meet a set of application requirements
- An understanding of security operations and risks 

### Exam Basics
- Category: Speciality (Pro-level difficulty)
- 170 minutes
- 65 questions (multiple choice or multiple response)
- Cost: 300 USD (150 with discount)

### Exam Domains and weightings:
- Domain 1: Threat Detection and Incident Response (14% of scored content)
- Domain 2: Security Logging and Monitoring (18% of scored content)
- Domain 3: Infrastructure Security (20% of scored content)
- Domain 4: Identity and Access Management (16% of scored content)
- Domain 5: Data Protection (18% of scored content)
- Domain 6: Management and Security Governance (14% of scored content)

### TD Recommended Whitepaper List:

#### AWS Security Whitepapers:
1. [Introduction to AWS Security](https://d1.awsstatic.com/whitepapers/Security/Intro_to_AWS_Security.pdf?did=wp_card&trk=wp_card)
2. [AWS: Overview of Security Processes](https://docs.aws.amazon.com/pdfs/whitepapers/latest/aws-overview-security-processes/aws-overview-security-processes.pdf)
3. [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
4. [Security Pillar – AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/welcome.html)
5. [AWS Security Best Practices](https://aws.amazon.com/architecture/security-identity-compliance)
6. [AWS Key Management Service Best Practices](https://d1.awsstatic.com/whitepapers/aws-kms-best-practices.pdf?did=wp_card&trk=wp_card)
7. [AWS Key Management Service Cryptographic Details](https://docs.aws.amazon.com/kms/latest/cryptographic-details/intro.html)
8. [Encrypting File Data with Amazon Elastic File System](https://docs.aws.amazon.com/whitepapers/latest/efs-encrypted-file-systems/efs-encrypted-file-systems.html)
9. [Secure Content Delivery with Amazon CloudFront](https://docs.aws.amazon.com/whitepapers/latest/secure-content-delivery-amazon-cloudfront/secure-content-delivery-with-amazon-cloudfront.html)
10. [Use AWS WAF to Mitigate OWASP's Top 10 Web Application Vulnerabilities](https://docs.aws.amazon.com/whitepapers/latest/guidelines-for-implementing-aws-waf/guidelines-for-implementing-aws-waf.html)
11. [Data Residency](https://d1.awsstatic.com/whitepapers/compliance/Data_Residency_Whitepaper.pdf?did=wp_card&trk=wp_card)
12. [AWS Best Practices for DDoS Resiliency](https://docs.aws.amazon.com/whitepapers/latest/aws-best-practices-ddos-resiliency/welcome.html)
13. [Application Logging in AWS](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/sec_detect_investigate_events_app_service_logging.html)
14. [AWS Security Incident Response Guide](https://docs.aws.amazon.com/whitepapers/latest/aws-security-incident-response-guide/aws-security-incident-response-guide.html)
15. [Best Practices for Security, Identity, & Compliance](https://aws.amazon.com/architecture/security-identity-compliance)

#### Compliance Whitepapers:
1. [AWS Security by Design](https://d1.awsstatic.com/whitepapers/compliance/Intro_to_Security_by_Design.pdf)
2. [AWS Risk & Compliance](https://d1.awsstatic.com/whitepapers/compliance/AWS_Risk_and_Compliance_Whitepaper.pdf?did=wp_card&trk=wp_card)
3. [Architecting for HIPAA Security and Compliance on AWS](https://docs.aws.amazon.com/whitepapers/latest/architecting-hipaa-security-and-compliance-on-aws/architecting-hipaa-security-and-compliance-on-aws.html)
4. [Navigating GDPR Compliance on AWS](https://docs.aws.amazon.com/whitepapers/latest/navigating-gdpr-compliance/welcome.html)
5. [Architecting for PCI DSS Scoping and Segmentation on AWS](https://d1.awsstatic.com/whitepapers/compliance/architecting-pci-dss-segmentation-scoping-aws.pdf)
6. [FedRAMP](https://aws.amazon.com/compliance/fedramp/)


### TD Recommended AWS Services to Focus On:

#### Identity and Access Control and AWS IAM Identity Center
- AWS Identity and Access Management (every detail)
- Resource-based Policies
- S3 Presigned URLs
- CloudFront signed URLs
- Amazon Cognito
- AWS IAM Identity Center
- AWS Security Token Service (STS)
- AWS Directory Service
- AWS Organizations
- AWS RAM (Resource Access Manager)

#### Application and Infrastructure Security
- EC2 key pairs
- AWS Systems Manager
- AWS WAF
- AWS Shield
- AWS Firewall Manager

#### Data Security
- AWS KMS
- Amazon CloudHSM
- AWS SSM Parameter Store
- Amazon Secrets Manager
- SSE-S3 Encryption
- S3 Glacier Vault Lock
- Amazon Macie
- AWS Certificate Manager

#### Network Security
- Amazon VPC
- Amazon CloudFront
- AWS ELB
- Amazon API Gateway
- AWS VPN
- AWS Direct Connect

#### Logging and Monitoring
- Amazon CloudWatch
- Amazon CloudTrail
- Service Logs (VPC, ELB, API Gateway, S3, CloudFront)
- Amazon Route 53
- Amazon GuardDuty
- Amazon Inspector
- Amazon Detective
- AWS Security Hub

#### Risk and Compliance Management
- AWS Artifact
- AWS Config

### Overview of study plan:
- 