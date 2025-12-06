# ArchHypo Patterns

# 📑 Table of Contents
- [Architectural Spike](#architectural-spike)
- [Architectural Trigger](#architectural-trigger)
- [Bring the Specialist](#bring-the-specialiste)
- [Continuous Inspection](#continuous-inspection)
- [Learning from Experiments](#learning-from-experiments)
- [Plan for Preparation](#plan-for-preparation)
- [Postpone Uncertain Decisions](#postpone-uncertain-decisions)
- [Protective Guideline](#protective-guideline)
- [Quality Checkpoint](#quality-checkpoint)
- [Software Analytics (What You Need to Know)](#software-analytics-what-you-need-to-know) 
- [Technical Debt Management](#technical-debt-management)
- [Tracer Bullets](#tracer-bullets)

---
## Architectural Spike
**Explanation:**

Used when there is technical uncertainty about an architectural solution. It involves developing a minimal and temporary implementation to explore the feasibility of a technology or approach, enabling quick learning without compromising the main project.

**Example:**

Before adopting WebAssembly to speed up parts of a web system, the team creates a simple prototype that runs a critical function and measures performance compared to JavaScript.

---

## Architectural Trigger
**Explanation:**

This pattern identifies events or changes that require architectural reassessment or decision-making. It could be a change in requirements, scaling needs, new regulations, or emerging technologies. Recognizing these triggers helps keep the architecture aligned with business goals.

**Example:**

The enforcement of the LGPD law requires the team to review the data architecture to ensure anonymization and explicit consent, triggering a decision about using privacy management services.

--- 

## Bring the Specialist
**Explanation:**

When the team faces a complex architectural decision or lacks expertise, this pattern recommends involving specialists — in security, AI, networking, or business domain — to ensure well-founded decisions and avoid technical risks.

**Example:**

When designing a facial recognition solution for access control, the team brings in a computer vision expert to define accuracy requirements and avoid algorithmic bias.

---
  
## Continuous Inspection
**Explanation:**

This pattern promotes continuous architectural review throughout the project lifecycle. It helps identify deviations, emerging risks, and improvement opportunities, keeping the architecture healthy and adaptable.

**Example:**

By implementing continuous monitoring of the architecture, with automated analysis of code quality, security vulnerabilities, and performance, the team can identify architectural, technical, and operational issues early, avoiding technical debt and production failures.

---
  
## Learning from Experiments
**Explanation:**

Suggests that architectural decisions be preceded by controlled experiments that generate real data and insights. This reduces risks and increases confidence in the chosen path.

**Example:**

The team tests three product recommendation models in test environments with real data to decide which offers the best accuracy and response time.

---

## Plan for Preparation
**Explanation:**

This pattern encourages preparing the architecture for future decisions, even if they are not yet mature. It includes creating flexibility, modularity, and abstractions that allow low-cost changes.

**Example:**

If we define in advance all activities, resources, tools, and responsibilities needed to start the project, we can ensure efficient preparation that minimizes risks, delays, and uncertainties during execution.

---

## Postpone Uncertain Decisions
**Explanation:**

When a decision involves many unknown variables or high risks, this pattern recommends postponing it until more information is available. This avoids premature decisions and allows incremental learning.

**Example:**

The team avoids choosing between containers or serverless for the backend until the request volume and usage profile become clearer after the MVP.

---

## Protective Guideline
**Explanation:**

Establishes architectural guidelines that protect the project from inconsistent decisions, inadequate techniques, or standard violations. These guidelines act as guardrails to maintain architectural integrity.

**Example:**

The team defines that all services must use OAuth2 authentication and that no external library can be used without a security review, preventing vulnerabilities.

---

## Quality Checkpoint
**Explanation:**

Creates specific moments to assess whether the architecture meets defined quality attributes (such as performance, security, scalability). These checkpoints help ensure technical goals are not compromised.

**Example:**

At each sprint delivery, the team runs automated load and security tests to validate that the system remains within acceptable latency and vulnerability limits.

---

## Software Analytics (What You Need to Know)
**Explanation:**

This pattern focuses on identifying knowledge gaps that hinder architectural decisions. It encourages actively seeking critical information through research, interviews, or data analysis.

**Example:**

Before defining the caching architecture, the team needs to know the average access time and data volume per session. They collect these metrics with the product team and real users.

---

## Technical Debt Management
**Explanation:**

This pattern deals with identifying, prioritizing, and mitigating technical debt accumulated throughout the project. Ignoring this debt can hinder architectural evolution and increase maintenance costs.

**Example:**

The team maintains a board with technical debts categorized by impact and effort and allocates part of the development time to eliminate the most critical ones, such as logic duplication or lack of test.

---

## Tracer Bullets
**Explanation:**

Minimal implementations that run through the system end-to-end, used to validate flows, integration, and overall architecture. They are useful for quickly testing hypotheses and ensuring components communicate correctly.

**Example:**

Before developing all modules of a reservation system, the team creates a basic flow from front-end to database, including authentication and API, validating the overall architecture.

---

ArchHypo.AI Plugin

Research and Development Team

[🔗 GitHub Repository](https://github.com/jonathancs-tester/ArchHypo-Trello-Plugin)
