# AI Lab Support and Campus Routing Assistant

> Assistant combining knowledge-base reasoning, constraint-based booking and shortest-path campus routing.

Built by **[Muhammad Tanveer](https://www.linkedin.com/in/muhammad-tanveer-advenno/)** - Full-Stack AI Automation Engineer.

[![Source](https://img.shields.io/badge/source-private%20repository-lightgrey)](#source-code-and-access) [![Role](https://img.shields.io/badge/built%20by-Muhammad%20Tanveer-blue)](https://github.com/haddindeve)

## Contents

- [The problem](#the-problem)
- [The approach](#the-approach)
- [Architecture](#architecture)
- [Tech stack](#tech-stack)
- [Key capabilities](#key-capabilities)
- [Selected code](#selected-code)
- [Results](#results)
- [FAQ](#faq)
- [Source code and access](#source-code-and-access)
- [About the engineer](#about-the-engineer)
- [Related projects](#related-projects)

## The problem

A campus assistant has to handle genuinely different question types - eligibility rules, room booking constraints, and navigation - each needing a different technique. One model cannot answer all three correctly.

## The approach

A router directs each request to the right technique: knowledge-base checks for eligibility, constraint satisfaction for booking feasibility, and weighted shortest-path search for navigation. Each answer comes from the method appropriate to it rather than from one general approximation.

## Architecture

| Component | Responsibility |
| --- | --- |
| **Request router** | Classification to the appropriate technique |
| **Knowledge base** | Rule-based eligibility checking |
| **CSP solver** | Booking constraint evaluation |
| **Graph routing** | Weighted shortest-path over the campus graph |
| **Templates** | Structured response formatting |

## Tech stack

| Layer | Technology |
| --- | --- |
| Language | Python |
| Techniques | Knowledge base, CSP, graph search |
| Testing | Automated test suite |
| Interface | Command-line demonstration |

## Key capabilities

- Request routing across reasoning techniques
- Rule-based eligibility validation
- Constraint-based booking checks
- Weighted campus shortest-path routing
- Structured response templates

## Selected code

From `ai_lab_support/__init__.py` in the private repository:

```python
"""AI Lab Support & Campus Routing package."""

from .core import CampusGraph, KnowledgeBase, Request, Router, build_default_router

__all__ = [
    "CampusGraph",
    "KnowledgeBase",
    "Request",
    "Router",
    "build_default_router",
]
```

## Results

- Each query class answered by the technique suited to it
- Deterministic, testable behaviour throughout

## FAQ

### Why several techniques instead of one model?

Eligibility, scheduling and routing are different computational problems. A rule base, a CSP solver and a graph search each answer their own correctly.

### What is the CSP used for?

Checking whether a requested booking satisfies all room, time and eligibility constraints simultaneously.

### How is routing calculated?

Weighted shortest-path search over a graph of campus locations.

### Is the code available?

Private repository.

## Source code and access

This repository is the public case study for **AI Lab Support and Campus Routing Assistant**. The full implementation - application code, database schema, tests and deployment configuration - lives in a **private repository** on this account, alongside the rest of the work shown here.

Source access can be arranged for hiring conversations, technical review or client due diligence. The quickest route is a short message on [LinkedIn](https://www.linkedin.com/in/muhammad-tanveer-advenno/) or an email to [mtanveertahir6666@gmail.com](mailto:mtanveertahir6666@gmail.com).

## About the engineer

**Muhammad Tanveer - Full-Stack AI Automation Engineer**

Full-stack AI automation engineer. I build agentic systems, browser and workflow automation, RAG pipelines and the production web platforms they run on - from Rust and Python services to Next.js dashboards and PHP/MySQL business systems.

- GitHub: [haddindeve](https://github.com/haddindeve)
- LinkedIn: [Muhammad Tanveer](https://www.linkedin.com/in/muhammad-tanveer-advenno/)
- Email: [mtanveertahir6666@gmail.com](mailto:mtanveertahir6666@gmail.com)
- Location: Pakistan

## Related projects

- [Gym Management CRM with NFC Gate Control](https://github.com/haddindeve/gym-management-crm-system)
- [Business OS - AI-Native Multi-Branch ERP](https://github.com/haddindeve/business-os-multi-branch-erp)
- [AuthentID - eMRTD Chip Identity Verification](https://github.com/haddindeve/authentid-emrtd-face-verification)
- [ARMenu - Augmented Reality Restaurant Menu SaaS](https://github.com/haddindeve/armenu-augmented-reality-menu-saas)
- [LinkedIn Lead Finder and Analyser](https://github.com/haddindeve/linkedin-lead-finder-and-analyser)
- [Offline-First Restaurant POS](https://github.com/haddindeve/restaurant-pos-offline-first)

---

<sub>AI Lab Support and Campus Routing Assistant - case study by Muhammad Tanveer - Full-Stack AI Automation Engineer. Keywords: AI assistant routing, constraint satisfaction problem, shortest path algorithm, knowledge base reasoning, campus navigation, academic AI project.</sub>