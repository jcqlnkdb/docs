# Project Report

## Overview

I built a documentation site for the TaskFlow API, covering onboarding, authentication, task management workflows, API behaviors, error handling, and endpoint reference documentation. The project was completed over approximately 12 hours across two days using Mintlify as the documentation platform. The final deliverable included both narrative documentation and structured API reference content designed for developers onboarding to the API for the first time.

---

## Editorial decisions and rationale

One of the main structural decisions was splitting the site into two clear navigation areas: **Documentation** and **API Reference**. This separated explanatory, workflow-oriented content from endpoint-level reference material, reducing cognitive overload for new users.

I also created a dedicated **Capabilities and Limitations** page because several API constraints were only implied in the specification rather than explicitly documented. Making these limitations visible helps reduce developer confusion and support overhead.

Another deliberate addition was an **API Behaviors** page documenting runtime behaviors that were observable during testing but not fully represented in the OpenAPI schema, such as validation patterns, status code expectations, and response conventions.

I distinguished between **Quickstart** and **Guides** intentionally:

* The Quickstart provides the minimum path to making a successful request.
* The Guides explain broader workflows and conceptual usage patterns.

For the API Reference itself, I relied on Mintlify's auto-generation capabilities from the OpenAPI specification, then enriched the generated content with contextual notes, warnings, and clarifications where necessary.

Throughout the site, I maintained a consistent editorial voice:

* second-person ("you")
* technical and direct language
* concise explanations
* no marketing-oriented phrasing

The goal was to make the documentation feel practical, trustworthy, and easy to scan.

---

## Process and methodology

I approached the project in phases to keep the work structured and avoid writing documentation before understanding the product behavior.

The first phase was discovery. I started by reading the OpenAPI specification in full, identifying the main entities, endpoint groups, authentication flow, and areas where the spec was ambiguous or incomplete. I also tested endpoints directly to understand runtime behavior beyond the static schema definitions.

Before writing, I created a lightweight information architecture and sitemap to define the separation between onboarding content, conceptual documentation, workflow guides, and API reference material. This helped avoid duplicated explanations and clarified what belonged in narrative documentation versus generated reference pages.

I prioritized the documentation in the following order:

1. Quickstart and onboarding flow
2. Core conceptual pages
3. Workflow guides
4. API behavior and limitations
5. Reference enhancements and error documentation
6. README and final review

I intentionally reserved time at the end for editorial review, consistency checks, navigation validation, and writing this report.

---

## Tools and AI assistance

### Documentation platform

The project was built using [Mintlify](https://mintlify.com) with the starter template as the foundation. The site was deployed using Mintlify's default subdomain to minimize deployment risk and reduce setup overhead during the limited project timeframe.

### API testing

For endpoint validation and behavior testing, I used Mintlify's built-in "Try It" functionality directly inside the documentation environment rather than setting up Postman or a separate API client. Given the time constraints, this was the most pragmatic workflow and allowed documentation and testing to happen simultaneously.

### AI assistance

I used [Claude](https://claude.ai) as a structured mentor throughout the project. Specifically:

* Crash courses on unfamiliar technical concepts, including REST conventions, OpenAPI structure, JSON syntax, Mintlify configuration, and MDX
* Editorial review of drafts for structure, hierarchy, clarity, parallelism, and scannability
* Validation of analytical decisions such as information architecture, page scope, and identification of gaps in the specification

Decisions regarding scope, editorial direction, voice, structure, prioritization, and final content were mine. Each page was initially drafted independently and then iteratively refined through feedback and revision.

The collaboration resembled the kind of mentorship process I would expect between a senior technical writer and a junior writer onboarding into a documentation team.

---

## What I learned

This project introduced me to several technical concepts and workflows that were new to me.

On the technical side, I learned:

* REST API conventions
* OpenAPI schema structure
* JSON formatting and validation
* HTTP methods and status codes
* documentation generation workflows

I also gained hands-on experience with:

* Mintlify
* MDX
* frontmatter configuration
* deployment workflows
* documentation site architecture

From a documentation perspective, I learned several common API documentation patterns, including:

* separating guides from reference material (a distinction articulated by frameworks such as Diátaxis)
* designing code-first quickstarts
* documenting behaviors beyond the schema
* using examples strategically
* prioritizing "show, don't tell" explanations

The project also reinforced the importance of documentation architecture as a UX problem, not just a writing exercise.

---

## What I would improve with more time

With additional time, I would expand and refine several areas of the project.

Potential improvements include:

* Custom visual branding, including TaskFlow-specific colors and logo integration
* More systematic testing of edge cases and error responses
* Code examples in multiple languages beyond cURL
* Visual diagrams, especially a Mermaid diagram illustrating the task lifecycle
* A dedicated "Glossary" or "Conventions" page for terminology and API patterns
* Local Mintlify CLI setup for faster iteration and preview workflows
* Accessibility review and usability testing with external readers
* Additional workflow tutorials for more advanced use cases

---

## Background

My academic background is in Journalism, with a Master's degree in Communication, alongside junior-level studies and practice in product design. These experiences strongly informed the documentation approach.

The journalism background influenced audience awareness, information prioritization, lead construction, and clarity and concision.

The communication research background contributed to analytical structuring, hierarchy decisions, consistency of tone, and attention to usability and readability.

My design studies informed navigation structure, scannability, progressive disclosure of information, and the separation between conceptual and operational content.

Together, these disciplines shaped both the editorial and UX decisions throughout the project.

---

## Time investment

Approximate time distribution:

* Discovery and setup: ~3h
* Writing core documentation pages: ~5h
* API Reference enrichment, errors, and behaviors: ~2h
* README and project report: ~1h
* Review, proofreading, and submission: ~1h

**Total:** approximately 12 hours.
