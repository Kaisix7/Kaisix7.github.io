# Working research plan

## Question

What security anti-patterns appear in sampled open-source React and Flutter repositories, and how reliably can existing static-analysis tools detect them?

## Boundaries

This is a proposal. No dataset has been collected, no vulnerability prevalence has been measured, and no paper has been accepted.

## Method to develop with a supervisor

1. Choose inclusion criteria and a documented sample of public repositories.
2. Define a taxonomy of security anti-patterns and the limits of detection.
3. Run reproducible scanner versions (for example, Semgrep or SonarQube when suitable).
4. Manually adjudicate a stratified sample to estimate false positives.
5. Report repository metadata, language differences, prevalence within the selected sample, and threats to validity.
6. Share code, selection criteria, and sanitized findings without exposing exploitable secrets or enabling unauthorized testing.
7. Write a research report or poster if evidence supports meaningful conclusions.

## Proposed capstone

*A Hybrid Vulnerability Analysis Framework for Modern Microservices Architecture*

Build an intentionally vulnerable local microservice application and compare source-based findings with controlled API testing. Track reproducibility, coverage, time spent on testing, precision, and false positives. Do not pre-write success percentages.

## Responsible testing

Use only her own systems, local intentionally vulnerable test applications, or systems for which explicit authorization has been obtained.
