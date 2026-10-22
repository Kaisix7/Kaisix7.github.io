---
layout: page
title: projects
permalink: /projects/
nav: true
nav_order: 3
description: A working collection of developer-facing security tools and experiments.
---

I want these projects to be more than attractive dashboards. Each one starts with a developer problem, a testable idea, and an honest account of what still needs work. **All three tools are in development.** Results and repositories will be added as implementations mature.

## CommitGuard

| | |
| :--- | :--- |
| **01 / DEVSECOPS** | **In development** |
| **Problem** | Secrets can reach a repository before anyone notices. Dependency warnings can be buried in noise. |
| **Approach** | Run small, explainable checks close to the commit and pull-request workflow. |
| **Planned stack** | Python · GitHub Actions · Docker · pattern matching |
| **What I'd like to measure** | Detection coverage, false positives, scan time, and how actionable the findings are. |

The first version will concentrate on credential patterns, dependency manifests, and readable reports. I'd rather produce one finding a developer understands than ten warnings they immediately dismiss.

**Planned evidence:** Test fixtures, sanitized CI logs, comparison with established scanners, and clearly documented limitations.

---

## FuzzRoute

| | |
| :--- | :--- |
| **02 / API SECURITY** | **In development** |
| **Problem** | REST endpoints often behave differently with unexpected input or incomplete authentication checks. |
| **Approach** | Read an OpenAPI definition and generate controlled tests against an isolated or explicitly authorized service. |
| **Planned stack** | Go or Node.js · OpenAPI · containerized test API |
| **What I'd like to measure** | Reproducible failures, endpoint coverage, noisy results, and missed edge cases. |

FuzzRoute starts from the API contract. I'm interested in how much useful coverage a specification can give us, where it leaves blind spots, and whether the tool can show developers enough context to reproduce an issue.

**Planned evidence:** A small intentionally vulnerable local API, saved request cases, and comparisons with existing API-testing tools.

---

## AuthAudit

| | |
| :--- | :--- |
| **03 / AUTHENTICATION** | **In development** |
| **Problem** | Authentication mistakes can hide in ordinary configuration and token-handling code. |
| **Approach** | Start with a narrow set of JWT and OAuth anti-patterns that can be tested reliably. |
| **Planned stack** | Python · AST parsing · Bash · unit tests |
| **What I'd like to measure** | Precision, false alarms, supported patterns, and situations static analysis cannot resolve. |

I'd like AuthAudit to explain why a pattern deserves attention rather than simply label it insecure. Understanding the limits of static checking is part of the work.

**Planned evidence:** Vulnerable/fixed examples, detection rules, and documented cases the checker does not understand.

---

## Graduation capstone

| | |
| :--- | :--- |
| **04 / PROPOSED THESIS · 2028** | **Subject to academic approval** |
| **Working title** | *A Hybrid Vulnerability Analysis Framework for Modern Microservices Architecture* |
| **Core idea** | Correlate static code-analysis findings with controlled dynamic API tests. |
| **Study design** | An isolated demonstration application, baseline scanners, reproducible issues, and evaluation of detection quality. |
| **What I'd like to learn** | Whether combining evidence helps prioritize genuine weaknesses and reduce duplicate alerts. |

This is a proposed graduation project, not a completed system. My aim is to develop something small enough to evaluate carefully but substantial enough to support a serious discussion of software security.

## How I document progress

| Build | Test | Explain |
| :--- | :--- | :--- |
| Working code and reproducible setup | Defined test cases and failure analysis | Limits, trade-offs, and results others can question |

You can follow the [research plan](/research/) and browse my [GitHub repositories](https://github.com/Kaisix7).
