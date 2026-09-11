# fortinet-nse-6-fortisoar-administrator-study-guide-
Complete community study guide, revision notes, hands-on lab scenarios, and study resources for the Fortinet NSE 6 FortiSOAR Administrator exam.
# Fortinet NSE 6 - FortiSOAR Administrator Study Guide

Welcome to the ultimate community-driven study guide for earning the **Fortinet NSE 6 - FortiSOAR Administrator** badge (and contributing toward the **Fortinet Certified Professional - Security Operations** track).

Whether you are a SOC analyst, security engineer, incident responder, or IT security architect, this repository provides a detailed, practical, and structured roadmap to master FortiSOAR deployment, administration, playbook orchestration, and multi-tenant security operations.

---

## 📌 Certification Overview

The **Fortinet NSE 6 - FortiSOAR Administrator** exam validates your ability to configure, manage, operate, and troubleshoot FortiSOAR in modern enterprise and multi-tenant SOC environments.

* **Exam Code:** NSE6_FSR-7.3 / FortiSOAR 7.x Administrator
* **Exam Provider:** Pearson VUE (Test Center or OnVUE Remote Proctoring)
* **Question Count:** ~30–35 questions (Multiple Choice & Drag-and-Drop)
* **Time Limit:** 60 minutes
* **Scoring:** Pass/Fail (Detailed performance report issued via Pearson VUE)
* **Prerequisites:** Minimum 6 months of hands-on experience managing FortiSOAR or SOC workflows recommended.

---

## 🎯 Who Should Take This Exam?

- **SOC Analysts & Engineers:** Professionals responsible for centralizing alert streams, managing incident queues, and automating triage workflows.
- **Incident Responders:** Engineers looking to standardize incident handling, create dynamic War Rooms, and execute automated mitigation playbooks.
- **Security Administrators & Consultants:** Technical leads deploying FortiSOAR instances, managing RBAC, handling high availability (HA), and integrating external security tools via connectors.

---

## 📊 Exam Objectives & Domain Breakdown

### Skills Measured & Domain Weights
| Domain | Description |
| :--- | :--- |
| **SOC and SOAR Overview** | Identify deployment requirements, license management, and initial environment initialization. |
| **System Configuration** | Configure system applications, custom fixtures, system proxy settings, audit logging, and import/export of modular configurations. |
| **Security Management** | Configure Role-Based Access Control (RBAC), team hierarchies, user authentication (Appliance vs. User), and troubleshoot security access issues. |
| **System Operation** | Externalize/migrate Elasticsearch indexes, configure recommendation engines, ML record similarity, and operate War Rooms. |
| **System Monitoring & HA** | Monitor system processes/services, review logs, manage multi-tenant environments, and configure High Availability (HA) clusters with PostgreSQL. |

---

## 🧠 Detailed Study Notes & Important Concepts

### Core Architecture & System Configuration
* **Deployment Models:** Understanding standalone, multi-tenant (Secure Message Exchange - SME), and High Availability (HA) cluster topographies.
* **Licensing & Initialization:** Managing license key activation, module entitlements, and environment customization (branding, system fixtures, time zones).
* **Configuration Portability:** Exporting and importing modular configuration packages across development, testing, and production instances.

### Security Management & Access Control
* **Role-Based Access Control (RBAC):** Defining fine-grained permissions across modules, records, and specific execution fields.
* **Team Hierarchies:** Designing team structures and inheritance models to delegate incidents across tiered SOC teams (Tier 1, Tier 2, Escalations).
* **Authentication Models:** Configuring local user accounts, LDAP/Active Directory integration, and SAML-based Single Sign-On (SSO).

### Search, Operations & Recommendation Engines
* **Elasticsearch Engine:** Managing record indexing, query optimizations, data retention, externalizing cluster indexes, and handling database growth.
* **Recommendation Engine & ML:** Configuring record similarity thresholds based on historical indicators (IPs, hashes, domain similarity) to highlight duplicate alerts automatically.
* **War Room Management:** Establishing real-time collaborative War Rooms for emergency incident response, linking relevant artifacts, execution tasks, and communication feeds.

### System Health, Monitoring & High Availability
* **High Availability (HA):** Configuring active-passive or active-active multi-node clusters backed by internal or external PostgreSQL databases and cluster licensing.
* **Service Monitoring:** Checking daemon states (Celery workers, PostgreSQL, Elasticsearch, RabbitMQ, and Nginx) using system tools and diagnostic logs.
* **Upgrades & Backup:** Preparing environment snapshots, executing database backups, and running automated CLI upgrade scripts.

---

## 🛠️ Practical Hands-on Exercises (Labs)

To build strong operational capabilities before taking the exam, complete these four hands-on scenario labs:

1. **Configure Role-Based Access Control (RBAC) and Teams:**
   * Create custom teams representing Tier 1 SOC Analysts and Incident Responders.
   * Define custom Roles restricting Tier 1 users to read/edit access on Alerts while restricting full Playbook execution to Tier 2 roles.
   * Test team inheritance and verify field-level record visibility.
2. **Deploy Connectors & Data Ingestion:**
   * Provision connectors from the FortiSOAR Content Hub (e.g., FortiGate, VirusTotal, or Active Directory).
   * Configure agent-based or direct API connectors and establish data ingestion schedules for Indicators of Compromise (IOCs).
   * Verify ingested logs in the Alert queue and validate automatic schema mapping.
3. **Configure High Availability (HA) with Cloud/External DB:**
   * Set up a secondary FortiSOAR node in a staging network.
   * Configure PostgreSQL database synchronization and cluster messaging via RabbitMQ.
   * Simulate a primary node failure and verify seamless cluster state failover.
4. **Establish Elasticsearch Similarity Matching:**
   * Configure the recommendation engine to evaluate incoming alert payloads against past incident records.
   * Fine-tune similarity weightings for IP addresses, file hashes, and target hostnames.
   * Validate that matching alerts generate contextual recommendations inside an active War Room.

---

## 📅 30-Day Exam Study Plan
