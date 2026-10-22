---
layout: page
title: projects
permalink: /projects/
nav: true
nav_order: 3
description: Security tools and software testing projects in development.
---

This is my working project log. I am building tools that help developers find security problems earlier, understand their causes, and make fixes easier to verify. I will add implementation links and test results as the projects progress.

## CommitGuard

**Status: In development** | **Area: DevSecOps and software supply-chain security**

A repository check for accidental secret exposure and risky third-party dependencies. The idea is to put useful feedback close to the development workflow, before insecure changes become difficult to trace.

**Planned stack:** Python, regular expressions, Docker, GitHub Actions.

**Planned work:** Secret-pattern detection, dependency manifest checks, structured findings, test fixtures, and a CI workflow that can fail safely when a high-confidence finding appears. False positives and exclusions will be recorded rather than hidden.

**Evidence to publish:** Test repositories, representative findings, CI logs, a threat model, and comparison against existing secret scanners.

---

## FuzzRoute

**Status: In development** | **Area: REST API security testing**

FuzzRoute is my plan for an API testing tool that reads an OpenAPI specification and generates controlled requests to find unexpected behavior. The first version will focus on parameter validation, unexpected status codes, authentication boundaries, and crash-resistant reporting.

**Planned stack:** Go or Node.js, OpenAPI, containerized test services.

**Planned work:** Parse specifications, generate constrained test cases, send requests only to owned or explicitly authorized test services, capture responses, and group reproducible findings.

**Evidence to publish:** An intentionally vulnerable local API, reproducible test cases, coverage information, and limitations compared with established API testing tools.

---

## AuthAudit

**Status: In development** | **Area: Authentication and source-code analysis**

A source-code checker for insecure JWT handling and common authentication mistakes. The project starts with a narrow set of patterns that can be tested precisely before expanding to other frameworks.

**Planned stack:** Python, AST parsing, Bash, unit tests.

**Planned work:** Identify missing token-expiration checks, incorrect algorithm validation, weak verification patterns, and risky configuration defaults in supported codebases.

**Evidence to publish:** Small vulnerable/fixed examples, detection rules, accuracy notes, and a clear explanation of unsupported patterns.

---

## Graduation capstone: hybrid vulnerability analysis

**Status: Proposed for 2028 graduation**

**Working title:** *A Hybrid Vulnerability Analysis Framework for Modern Microservices Architecture*

The proposed capstone would connect static findings from application code with observations from controlled dynamic API tests. I want to study whether connecting those two forms of evidence helps developers prioritize reproducible weaknesses.

The planned evaluation includes an intentionally vulnerable demonstration service, baseline scanners, controlled experiments, and measured false-positive rates. Any performance claims will depend on collected results rather than assumptions.

**Research direction:** Secure software architecture, static and dynamic testing, vulnerability triage.
