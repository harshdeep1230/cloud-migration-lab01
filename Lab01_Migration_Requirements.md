# Lab 01 – Migration Requirements Gathering

## 1. Case Study Overview

- **Company name:** :ASOS
- **Industry:** E-commerce / Online Retail
- **Existing environment:** Primarily on-premises infrastructure with legacy systems supporting a rapidly growing global e-commerce platform
- **Target cloud platform:** Microsoft Azure

ASOS is a online fashion retailer with a global reach which is growing at a very high rate and has very fluctuating traffic pattern. Its on-premises infrastructure was not able to scale effectively in times of peak shopping, and it switched to Microsoft Azure.
---

## 2. Company Motivations for Cloud Migration

The primary motivations for ASOS to migrate to the cloud include:

- **Scalability:** The need to handle significant traffic spikes during sales and seasonal events without over-provisioning hardware
- **Reliability and availability:** Reducing downtime and improving system resilience to protect revenue and customer trust
- **Faster deployment:** Enabling quicker release cycles and more agile development practices
- **Cost optimization:** Shifting from capital expenditure on physical infrastructure to a pay-as-you-go cloud model
- **Global performance:** Leveraging Azure’s global regions and content delivery capabilities to improve user experience worldwide

---

## 3. Infrastructure Discovery Questions

To fully understand ASOS’s existing environment, the following questions must be addressed before migration:

- How many servers and virtual machines are currently in use, and what workloads do they support?
- What operating systems and software versions are running across the environment?
- Which applications are business-critical and require high availability?
- What dependencies exist between applications and services?
- What is the acceptable downtime for each system during migration?
- Does the internal IT team have experience managing Azure environments?

---

## 4. RACI Matrix

| Role                | Responsibility |
|---------------------|----------------|
| Project Manager     | Accountable    |
| Cloud Architect     | Responsible    |
| IT Operations Team  | Responsible    |
| Security Team       | Consulted      |
| Business Owner      | Informed       |
| Azure Vendor Support| Consulted      |

---

## 5. Migration Approach

A **rehost and replatform** migration approach is the most suitable for ASOS.

Rehosting (lift-and-shift) allows ASOS to migrate existing workloads quickly with minimal changes, reducing risk and downtime

---

## 6. High-Level Migration Schedule

- **Weeks 1–2:** Infrastructure assessment and requirements gathering
- **Weeks 3–4:** Pilot migration of non-critical workloads
- **Weeks 5–6:** Migration of core e-commerce systems
- **Week 7:** Testing, validation, and performance optimization
- **Week 8:** Production go-live and post-migration monitoring

---

## 7. Decision Criteria

The main decision criteria for ASOS’s cloud migration include:

- Ability to scale infrastructure dynamically during peak demand
- Minimal downtime and business disruption during migration
- Compliance with security and regulatory standards

