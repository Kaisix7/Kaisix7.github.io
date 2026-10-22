# Karina Baitenova

**Software Engineering student | Secure Software Systems | Application Security**

*I like building software. I am even more interested in understanding where it breaks, and how to make it safer before anyone depends on it.*

[![Portfolio](https://img.shields.io/badge/Portfolio-Explore_my_work-183A37?style=for-the-badge)](https://kaisix7.github.io/)
[![GitHub](https://img.shields.io/badge/GitHub-Kaisix7-20242B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Kaisix7)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karina-b-a022311b1x)


---

## A little about me

I'm Karina, a Software Engineering student at AlmaU, currently studying in the Russian-language group and expecting to graduate in **2028**.

Building applications has made me curious about the decisions developers make long before a security problem becomes visible. How are permissions checked? What happens when an API receives input nobody expected? Can a testing tool catch a mistake while the code is still being written?

Those are the questions shaping my interest in **secure software engineering, application security, vulnerability analysis, and DevSecOps**. I also want to explore where applied AI can make software testing and security analysis more useful, without treating a model's answer as proof that something is safe.

I'm still learning and building. This space is where I document that process, including the approaches that work, the ones I have to rethink, and the questions I have not answered yet.

## On my workbench

These are my **current project directions**, not claims of finished products. As the implementations develop, I'll add code, tests, examples, and measurements to their own repositories.

| Project | What I'm working toward | Questions I'm exploring |
| :--- | :--- | :--- |
| **CommitGuard** | A developer-focused checker for accidentally committed secrets and insecure dependency choices, designed for CI workflows. | How much risk can a lightweight pre-merge check catch without burying developers in false alarms? |
| **FuzzRoute** | An OpenAPI-driven REST API testing tool for controlled, authorized test environments. | Can API specifications help generate meaningful edge cases, not just random requests? |
| **AuthAudit** | A source-analysis tool for spotting risky JWT and OAuth configuration patterns. | How can a scanner distinguish dangerous authentication mistakes from harmless implementation differences? |

I intend to use Python, GitHub Actions, containers, and relevant API-testing tools where they fit. The tools and scope may change as I prototype and evaluate each idea.

**Research and project pages:** [Projects](https://kaisix7.github.io/projects/) · [Research](https://kaisix7.github.io/research/) · [Repositories](https://kaisix7.github.io/repositories/)

## A problem I want to study

**Security anti-patterns in open-source React and Flutter applications**

I want to investigate which security mistakes appear repeatedly in public applications and whether automated analysis can identify them with enough context to be useful.

My proposed approach is to select a reproducible sample of suitable repositories, apply documented static-analysis rules, manually validate a subset of the findings, and report the limitations as carefully as the results.

This is a **research proposal**, not a published paper or a completed study. A good result would be a method someone else can reproduce and a set of findings that do not overstate what automated scanners can prove.

## The graduation project I'm aiming for

### A hybrid vulnerability analysis framework for microservices

My proposed capstone would bring static code analysis and dynamic API testing into one workflow.

The plan is to build a small, deliberately vulnerable test application, analyze its code, test its running endpoints in an isolated environment, and correlate findings to reduce duplicate reports. I also want to study what the combined approach misses and how much effort is needed to verify a finding.

It is a proposal I hope to develop into a graduation project, subject to academic approval and the practical scope I can complete.

## Looking toward 2028

After graduation, I hope to move directly into graduate study without taking a planned gap year. I'm exploring **English-taught Master's programs** in Information Security, Security Informatics, Applied Artificial Intelligence, and Software Engineering, as well as **direct-entry PhD paths in Computer Science** where my preparation and the admissions requirements align.

I am especially drawn to research groups working on software security, automated testing, program analysis, and dependable systems. Funding, supervisor fit, and the opportunity to do rigorous work will matter more to me than an impressive program title alone.

My near-term priorities are straightforward: build tools I can explain line by line, test them against realistic cases, document their limitations, and develop a research question worth pursuing seriously.

## Research identity & connections

[![ResearchGate](https://img.shields.io/badge/ResearchGate-Research_profile-00CCBB?style=flat-square&logo=researchgate&logoColor=white)](https://www.researchgate.net/profile/Karina-Baitenova)
·
[![ORCID](https://img.shields.io/badge/ORCID-0009--0003--4256--6862-A6CE39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0003-4256-6862)
·
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Karina_B.-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karina-b-a022311b1x)
·
[![GitHub](https://img.shields.io/badge/GitHub-Kaisix7-20242B?style=flat-square&logo=github&logoColor=white)](https://github.com/Kaisix7)


> I value thoughtful reviews, reproducible experiments, and feedback that makes a piece of software genuinely better. If you're working on secure development, testing, or software security research, I'd be glad to connect.

---

## About this website and repository

This repository contains my academic portfolio, built with **Jekyll 4.4** and **al-folio v1.0.15**. The theme and configuration started from an existing customized portfolio shared with permission, then were adapted to my own writing, design choices, and research direction.

- [`about.md`](about.md): background and interests
- [`projects.md`](projects.md): projects in development and capstone proposal
- [`research.md`](research.md): research questions and graduate interests
- [`publications.md`](publications.md): publication status; no invented citations
- [`repositories.md`](repositories.md): code and experiments
- [`blog.md`](blog.md): occasional engineering notes
- [`cv.md`](cv.md): academic CV page
- [`SETUP_FOR_KARINA.md`](SETUP_FOR_KARINA.md): photo replacement and deployment checks

### Local development

```bash
bundle install
bundle exec jekyll doctor
bundle exec jekyll build --trace
bundle exec jekyll serve --host 0.0.0.0 --port 4000 --force_polling --watch
```

The original theme is [al-folio](https://github.com/alshedivat/al-folio). Its licenses and any third-party notices should remain intact.


  *Built one experiment, one review, and one better question at a time.*
