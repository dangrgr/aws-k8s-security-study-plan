# 🧠 AWS + Kubernetes Security Study Plan — Structured (17 Weeks)

This plan blends three learning tracks:
1. AWS Certified Security Specialty (SCS-C02)
2. Offensive AWS skills (ACRTP)
3. Kubernetes security ( *Hacking Kubernetes* book)

> **Tracking:** Each week ends with a *Deliverables* list. Record these in `progress.md` (or GitHub Issues) and attach artifacts (screenshots, notes). Aim to complete ≥ 90 % of deliverables before moving on.
>
> **Time Estimates:** Rough hours help you gauge workload. Adjust as needed based on personal pace.

## 📅 High-Level Timeline

| Date | Week | Major Milestone |
|------|------|-----------------|
| 2025-07-31 | Week 1 | Kick-off & Baseline mock exam |
| 2025-08-07 | Week 2 | IAM focus |
| 2025-08-14 | Week 3 | Data protection (KMS/S3) |
| 2025-08-21 | Week 4 | Serverless & IaC attack paths |
| 2025-08-28 | Week 5 | EKS foundations + CIS benchmark |
| 2025-09-04 | Week 6 | Detection & logging enablement |
| 2025-09-11 | Week 7 | FLEX buffer / catch-up |
| 2025-09-18 | Week 8 | Advanced EKS attacks + GuardDuty runtime |
| 2025-09-25 | Week 9 | Network Firewall, Firewall Manager, Macie, threat intel |
| 2025-10-02 | Week 10 | AWS Cyber Range (2-day) |
| 2025-10-09 | Week 11 | Mock exam 1 (≥75 %) |
| 2025-10-16 | Week 12 | Mock exam 2 (≥80 %) |
| 2025-10-23 | Week 13 | Final review & AWS SCS-C02 exam (target) |
| 2025-10-30 | Week 14 | Electra Range mock exam |
| 2025-11-06 | Week 15 | ACRTP attempt #1 (24 h) |
| 2025-11-13 | Week 16 | Post-exam analysis & retake prep |
| 2025-11-20 | Week 17 | **(Optional)** ACRTP retake / bonus research |

---

## Week 1 — 2025-07-31   Baseline & Kick-off  (~8–10 h)

### Goals
1. Review AWS Security Specialty exam guide (SCS-C02)
2. Baseline self-assessment using TD mock exam (test all domains)
3. Schedule ACRTP exam & choose AWS Cyber Range track
4. Set up lab environment (IAM, S3, Lambda basics)

### Weekend Catch-up Plan
- **Saturday**: Analyze mock results, identify weak areas, review TD explanations
- **Sunday**: Schedule ACRTP exam, choose Cyber Range track, AND lab environment setup with Terraform bootstrap

### Daily Breakdown
| Day | Activity | Est. hrs |
|-----|----------|----------|
|Thu  | Skim exam guide & outline domain weights | 1.5 |
|Fri  | Take baseline mock exam (Timed, 65 Q) | 2 |
|Sat  | Analyse mock results; log weak areas | 1 |
|Sun  | Schedule ACRTP exam, Pick Cyber Range track, Build lab AWS account + Terraform bootstrap | 3.5 |

### Deliverables / Metrics
- Baseline mock-exam score recorded (target ⩾ 50 %) ✅ **67.69% - EXCEEDED!**
- ACRTP & Cyber Range dates booked
- `lab-bootstrap/` repository pushed; screenshot of successful `terraform apply`
- Week-1 recap note (≥ 250 words) committed
- Knowledge gaps analysis completed and documented

---

## Week 2 — 2025-08-07   Identity & Access   (~9 h)

### Goals
1. Read Tutorials Dojo Domain 1: Identity & Access Management (sections 1.1-1.4)
2. Watch Cantrill IAM videos + take notes
3. Complete ACRTP IAM PrivEsc chain lab
4. Review IAM JSON policy evaluation logic
5. Read AWS IAM best-practices whitepaper

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 1.1-1.2: IAM fundamentals + SCPs + Cantrill IAM 101–201 videos|2.5|
|Tue|TD Domain 1.3-1.4: Advanced IAM + Cantrill IAM advanced scenarios|2|
|Wed|ACRTP IAM PrivEsc lab (hands-on)|3|
|Thu|Read IAM policy evaluation blog; build test cases|1|
|Fri|Whitepaper skim & notes; recap|0.5|

### Deliverables / Metrics
- Lab report showing PrivEsc chain & mitigation
- 5 custom IAM policy examples pushed to `iam-playground/`
- TD IAM practice-set score recorded (target ≥ 70 %)
- Key-takeaways bullet list (#IAM tag) appended to `notes.md`

---

## Week 3 — 2025-08-14   Data Protection (KMS, S3)   (~9 h)

### Goals
1. Read Tutorials Dojo Domain 2: Data Protection (sections 2.1-2.4)
2. Watch Cantrill KMS/S3 security videos
3. Perform ACRTP S3 Enumeration and KMS key-access labs
4. Lab: S3 access controls, encryption at rest vs. in transit
5. Study envelope encryption & key policies

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 2.1-2.2: KMS fundamentals (key rotation, types) + Cantrill KMS intro & demos|2|
|Tue|TD Domain 2.3-2.4: S3 security (encryption types, bucket policies) + Cantrill S3 security module|2|
|Wed|ACRTP S3 Enumeration lab|2|
|Thu|Lab: S3 ACL vs. bucket policy vs. IAM|2|
|Fri|Deep-dive on envelope encryption; write summary|1|

### Deliverables / Metrics
- S3/KMS lab artefacts & screenshots
- Table comparing SSE-S3, SSE-KMS, CSE
- TD Data Protection practice-set score recorded (target ≥ 70 %)
- 250-word weekly recap committed

---

## Week 4 — 2025-08-21   Serverless & Infrastructure Attack Paths  (~10 h)

### Goals
1. Read Tutorials Dojo Domain 3: Infrastructure Security (sections 3.1-3.3)
2. ACRTP Lambda privilege-escalation lab
3. Watch Cantrill Lambda security content
4. Review CloudFormation drift & misconfig issues
5. Explore IaC scanners (cfn-nag, Checkov)

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 3.1: Lambda security + Cantrill Lambda security videos|2.5|
|Tue|TD Domain 3.2-3.3: Infrastructure security (VPC endpoints) + ACRTP Lambda PrivEsc lab|3|
|Wed|CloudFormation drift & audit demo|1.5|
|Thu|Run cfn-nag/Checkov against sample stacks|2|
|Fri|Blog post: "Top 5 Lambda attack vectors"|1|

### Deliverables / Metrics
- Lambda PrivEsc chain write-up & patched policy
- IaC scan report (cfn-nag / Checkov) stored in `/reports/`
- Weekly recap note committed

---

## Week 5 — 2025-08-28   EKS Security Foundations + Hacking K8s Ch. 1–5  (~10 h)

### Goals
1. Read Tutorials Dojo Domain 3: Container Security (sections 3.4-3.5)
2. Intro to Kubernetes attack surface
3. Lab: Create EKS cluster with IRSA; test pod role assumptions
4. Read chapters 1–5 of *Hacking Kubernetes*
5. Review IRSA, OIDC providers, and pod-level IAM
6. Run CIS-EKS benchmark (`kube-bench`) baseline scan

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 3.4-3.5: Container security + Create EKS cluster + IRSA set-up|2.5|
|Tue|Test pod role assumption; demo IRSA|2|
|Wed|Read Hacking K8s Ch.1–2 + notes|1.5|
|Thu|Read Ch.3–5|1.5|
|Fri|Run `kube-bench`; draft hardening checklist|2|

### Deliverables / Metrics
- `eks/cluster.tf` & IRSA YAML committed
- `kube-bench` JSON report stored
- Initial EKS hardening checklist pushed

---

## Week 6 — 2025-09-04   AWS Detection & Logging  (~9 h)

### Goals
1. Read Tutorials Dojo Domain 4: Threat Detection & Incident Response (sections 4.1-4.3)
2. Configure & test GuardDuty, CloudTrail, Security Hub
3. Watch Cantrill logging & monitoring modules
4. ACRTP detection-evasion lab
5. Enable AWS Config & Detective; explore findings

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 4.1: Threat detection + Enable CloudTrail + GuardDuty baseline|2|
|Tue|TD Domain 4.2-4.3: Incident response + Enable Security Hub + Detective integrations|2|
|Wed|Cantrill videos on detection & logging|2|
|Thu|ACRTP detection-evasion lab|2.5|
|Fri|Review Config rules; weekly recap|0.5|

### Deliverables / Metrics
- GuardDuty & Detective findings screenshot bundle
- CloudTrail + Config configuration committed (Terraform)
- TD Threat Detection practice-set score recorded (target ≥ 75 %)
- Lab report: techniques that evaded detection vs. caught

---

## Week 7 — 2025-09-11   FLEX BUFFER / CATCH-UP

> Use this week to: finish outstanding deliverables, revisit confusing topics, or deepen lab work. If fully caught up, choose an elective mini-project (e.g., automate GuardDuty → Slack alerts).

### Suggested Activities
- **TD Review**: Re-read weak domains from Tutorials Dojo guide
- Close any *open* GitHub issues from Weeks 1–6
- Re-take baseline mock exam; compare score change
- Polish notes; generate flashcards for weak domains
- Rest or pursue mini-project (max 6 h)

### Deliverables
- Outstanding deliverables marked **Done**
- Mini-project PR merged (optional)

---

## Week 8 — 2025-09-18   Advanced EKS Attacks + Hacking K8s Ch. 6–9  (~10 h)

### Goals
1. Read Tutorials Dojo Domain 4: Advanced Threat Detection (sections 4.4-4.5)
2. Lab: Pod escape, kubelet abuse, RBAC escalation
3. Read chapters 6–9 of *Hacking Kubernetes*
4. Enable GuardDuty EKS **Runtime Monitoring**; simulate detections
5. Review AWS Inspector results for EKS workloads

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 4.4-4.5: Advanced detection + Read Hacking K8s Ch.6–7|2|
|Tue|Read Ch.8–9|1.5|
|Wed|Lab: Pod escape & RBAC escalation|3|
|Thu|Enable GuardDuty EKS Runtime Monitoring; generate test findings|2|
|Fri|Inspect Inspector reports; weekly recap|1.5|

### Deliverables / Metrics
- Attack demo scripts pushed to `eks-attacks/`
- GuardDuty EKS runtime findings screenshot bundle
- Weekly recap note committed

---

## Week 9 — 2025-09-25   Network Firewall, Firewall Manager, Macie + Threat Intel  (~8 h)

### Goals
1. Read Tutorials Dojo Domain 5: Management & Governance (sections 5.1-5.3)
2. Deploy AWS Network Firewall in a sandbox VPC; write Suricata rule to block malicious traffic
3. Configure AWS Firewall Manager policy to enforce SG baseline across accounts
4. Run Macie discovery scan & create EventBridge->Lambda auto-remediation for public S3
5. Skim MadPot IOCs & other threat-intel feeds; update NF Suricata rules

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 5.1-5.2: Governance + Watch Cantrill DDoS & Network Firewall overview|2|
|Tue|TD Domain 5.3: Management + Deploy Network Firewall; craft & test Suricata rule|2.5|
|Wed|Set up Firewall Manager SG baseline policy and evaluate|1.5|
|Thu|Run Macie scan; build Lambda auto-remediation for public objects|1|
|Fri|Ingest MadPot IOCs; update NF rules; weekly recap|1|

### Deliverables / Metrics
- Network Firewall JSON policy & Suricata rule committed
- Firewall Manager policy screenshot bundle
- Lambda remediation code stored in `automation/`
- Macie findings report uploaded

---

## Week 10 — 2025-10-02   AWS Cyber Range   (~full-time week, 30+ h)

### Goals
1. Complete chosen AWS Cyber Range (Detection or Incident Response)
2. Take notes on workflow, response triage, automation hooks
3. Link EKS logs or findings back to GuardDuty/Security Hub

### Daily Breakdown
> Cyber Range schedules vary; block two full days for scenarios.

### Deliverables / Metrics
- Cyber Range completion certificate (PDF) stored
- Incident timeline notes committed
- PR: Automation script integrating EKS logs → Security Hub (optional)

---

## Week 11 — 2025-10-09   Exam Review — IAM, KMS, Detection   (~7 h)

### Goals
1. Read Tutorials Dojo Domain 6: Application Security (sections 6.1-6.2)
2. Mock exam 1 (full TD practice test) — review & analyse
3. Flashcards + cheat-sheet review (focus: IAM/KMS/S3)
4. Lab revisit: IAM & KMS misconfigs and fixes
5. Write concise notes for rapid recall

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 6.1-6.2: Application security + Take Mock exam 1|3|
|Tue|Analyse wrong answers|1.5|
|Wed|Flashcards review|1|
|Thu|Lab revisit & patch misconfigs|1.5|
|Fri|Summarise notes; recap|0|

### Deliverables / Metrics
- Mock exam 1 (TD full-length) score ≥ 75 %
- Updated cheat sheet committed

---

## Week 12 — 2025-10-16   Exam Review — Containers, Serverless, Edge   (~7 h)

### Goals
1. Read Tutorials Dojo Domain 6: Advanced Application Security (sections 6.3-6.4)
2. Mock exam 2 (TD full practice test #2) — track progress
3. Focus areas: Lambda, EKS, WAF, CloudFront, IRSA
4. Summarise key Kubernetes attack paths
5. Triage weaknesses from mock review

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Domain 6.3-6.4: Advanced app security + Mock exam 2|3|
|Tue|Analyse results|1.5|
|Wed|Lambda & CloudFront flashcards|1|
|Thu|EKS attack-path mind-map|1.5|
|Fri|Triage doc + recap|0|

### Deliverables / Metrics
- Mock exam 2 (TD full-length) score ≥ 80 %
- Kubernetes attack-path mind-map image committed

---

## Week 13 — 2025-10-23   Final Review + Exam Week   (~5 h + exam day)

### Goals
1. Read Tutorials Dojo: Full Review & Exam Strategies (final sections)
2. Mock exam 3 — final pass
3. Re-watch select Cantrill videos (weak areas only)
4. Skim all flashcards once
5. Rest, test readiness, sit for exam!

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|TD Final Review + Mock exam 3|3|
|Tue|Video rewatch (targeted)|1.5|
|Wed|Flashcard blitz|1|
|Thu|Light rest / walk-through notes|0.5|
|Fri|Exam day 🎉|

### Deliverables / Metrics
- Mock exam 3 score ≥ 85 %
- Exam passed ✅ (celebrate!)

---

## Week 14 — 2025-10-30   Electra Range Mock Exam  (~12 h)

### Goals
1. Complete the Electra AWS cyber range (9 flags)
2. Simulate full ACRTP workflow: enumeration → exploitation → evidence gathering
3. Produce a short engagement report (≤ 5 pages)
4. Refine tooling/environment ahead of ACRTP exam

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|Read Electra scenario & prep notes|2|
|Tue|Electra range exploitation (phase 1)|4|
|Wed|Electra range exploitation (phase 2) + flag capture|3|
|Thu|Compile evidence & draft mini-report|2|
|Fri|Identify tooling gaps; update scripts|1|

### Deliverables / Metrics
- 9 Electra flags captured (screenshots)
- 5-page engagement report committed to `electra-report/`
- Updated helper scripts & tooling checklist

---

## Week 15 — 2025-11-06   ACRTP Attempt #1 (24-Hour Practical)  (full-time, 30+ h)

### Goals
1. Complete ACRTP exam within the 24-hour window
2. Produce and submit the required exam report
3. Log time spent per objective for post-mortem

### Schedule
| Day | Activity |
|-----|----------|
|Thu 00:00 | Exam window opens – enumeration & note-taking |
|Thu daylight | Exploitation & privilege escalation |
|Fri early AM | Cleanup, screenshots, evidence collection |
|Fri daytime | Draft report & proof-of-concept scripts |
|Fri evening | Finalise & submit report |

### Deliverables / Metrics
- ACRTP exam report submitted on time ✅
- Self-logged objective completion table stored in `acrtp-exam/`
- Quick retro notes (what worked / what didn’t) committed

---

## Week 16 — 2025-11-13   Post-Exam Analysis & Retake Prep  (~6 h)

### Goals
1. Review ACRTP #1 results & feedback (pass/fail)
2. If passed: summarise take-aways and plan next learning path
3. If failed: identify top gaps and craft remediation plan for retake
4. Update tooling/scripts based on exam experience

### Daily Breakdown
|Day|Activity|hrs|
|---|--------|---|
|Mon|Analyse exam results & feedback|2|
|Tue|Targeted remediation labs / note writing|2|
|Wed|Prepare retake checklist **or** draft lessons-learned blog|2|

### Deliverables / Metrics
- Pass scenario: 500-word blog/internal post & updated roadmap
- Fail scenario: Remediation checklist + updated scripts committed

---

## Week 17 — 2025-11-20   **Optional** ACRTP Retake / Bonus Research  (variable hours)

### Goals
*Retake path*
1. Complete ACRTP retake exam within the 24-hour window
2. Submit exam report & log time per objective

*Bonus-research path (if passed)*
1. Deep-dive elective topic (e.g., advanced IAM exploitation or EKS network hardening)
2. Craft conference-style write-up or tooling improvement

### Deliverables / Metrics
- Retake: exam report submitted ✅
- Research: publish 1000-word article/tool PR

---

## 🔖 Reference & Tracking Tips

1. **GitHub Projects (Kanban):**
   - Columns: *Backlog*, *This Week*, *In Progress*, *Done*.
   - Create an *Issue* for every deliverable; link PRs/commits.
2. **Weekly Recap Notes:** Commit a `week-N.md` recap every Friday containing:
   - Key take-aways
   - Hours actually spent vs. estimate
   - Blockers & next-week focus
3. **Progress Badges:** Add shields.io badges (e.g., completed / total weeks) to `README.md`.
4. **Automated Metrics:**
   - Use GitHub Actions to count completed issues and update a progress graph.
5. **Peer Review / Share-outs:** Schedule a 30-min sync every 3–4 weeks to explain what you’ve learned. Teaching reinforces retention.
6. **Health & Burnout:** Insert mini-breaks (walk, exercise, hobby) each day; Week 7 is a full buffer.

Good luck—stick to the structure, adapt when real life intervenes, and you’ll be exam-ready in thirteen productive weeks! 🎯
