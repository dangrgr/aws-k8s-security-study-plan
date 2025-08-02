# Knowledge Gaps Tracker

## Current Gaps

### Data Protection Domain (Priority: HIGH - 37.5% performance)

#### KMS Key Management & Rotation
- **Gap**: Understanding KMS key types and automatic rotation limitations
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**: 
  - Customer-managed symmetric keys DO support automatic rotation (missed on Q23)
  - Imported key material and custom key stores do NOT support automatic rotation (Q54)
  - Asymmetric KMS keys do NOT support automatic rotation (Q54)
- **Plan**: Focus Week 3 KMS labs, review TD Data Protection section

#### Envelope Encryption & Encryption Context
- **Gap**: Understanding envelope encryption process and encryption context
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - Envelope encryption: encrypt data with data key, then encrypt data key with master key (Q50)
  - EncryptionContext vs AuthenticationContext in DynamoDB (Q55)
  - EncryptionContext requires additional info (email/username) for decryption
- **Plan**: Deep dive in Week 3, hands-on KMS labs

#### S3 Security & Access Controls
- **Gap**: S3 bucket policies, encryption types, and access patterns
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - SSE-S3 vs SSE-KMS vs SSE-C differences (Q27)
  - S3 bucket policies with aws:SourceIp and aws:sourceVpc conditions (Q8)
  - GuardDuty S3 Protection finding types (Q9)
- **Plan**: Week 3 S3 labs, review TD S3 security section

#### EFS Encryption & Key Rotation
- **Gap**: EFS encryption requirements and key management
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - Cannot enable encryption on existing unencrypted EFS (Q6)
  - Must create new EFS with KMS customer-managed key for rotation
- **Plan**: Week 3 storage security review

### Threat Detection Domain (Priority: MEDIUM)

#### CloudTrail & CloudWatch Integration
- **Gap**: Setting up CloudTrail with CloudWatch for monitoring
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - CloudTrail → CloudWatch Logs → Metric Filter → Alarm pattern (Q65)
  - Route 53 DNS query logging vs Resolver query logging (Q46)
- **Plan**: Week 6 detection & logging focus

#### GuardDuty & Security Hub Integration
- **Gap**: Understanding service integration and finding types
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - AWS Config + Security Hub for CIS benchmarks (Q2)
  - GuardDuty S3 Protection finding types (Q9)
- **Plan**: Week 6 hands-on labs

### Infrastructure Security Domain (Priority: MEDIUM)

#### VPC & Network Security
- **Gap**: VPC endpoints, security groups, and network access
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - VPC Interface endpoints for Systems Manager (Q20)
  - Security group rules for private subnets (Q44)
  - Port 587 for SMTP with TLS (Q40)
- **Plan**: Week 2 network security review

#### EC2 Security & Metadata Service
- **Gap**: EC2 instance metadata service security
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - IMDSv1 vs IMDSv2 security (Q15)
  - Cannot disable metadata service via SSM Agent
- **Plan**: Week 2 EC2 security labs

### Identity & Access Management Domain (Priority: LOW - Strong performance)

#### SCPs & IAM Policy Evaluation
- **Gap**: Understanding SCP precedence and policy evaluation
- **Identified**: 2025-08-01 (Baseline mock exam)
- **Status**: Active
- **Details**:
  - SCPs must explicitly allow actions (Q59)
  - SCPs don't support whitelisting (Q59)
- **Plan**: Week 2 IAM policy review

## Resolved Gaps

### None yet - just started study plan

## Action Items

### Immediate (This Week)
1. **Review TD explanations** for all missed Data Protection questions
2. **Skim Tutorials Dojo Data Protection section** to identify key concepts
3. **Focus Week 3 preparation** on KMS, S3, and envelope encryption

### Week 2 Adjustments
1. **Add 30 minutes** to IAM day for SCP policy evaluation review
2. **Add 30 minutes** to network security day for VPC endpoints

### Week 3 Focus Areas
1. **KMS key types and rotation** (high priority)
2. **Envelope encryption process** (high priority)
3. **S3 encryption types and policies** (high priority)
4. **EFS encryption requirements** (medium priority) 