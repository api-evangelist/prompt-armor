# PromptArmor (prompt-armor)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

PromptArmor (YC W24) is an LLM application security platform that detects and blocks enterprise-grade threats - indirect prompt injection, data exfiltration, phishing, and system manipulation - in production AI applications. A real-time detection API analyzes LLM inputs and outputs against a continuously updated set of threat detectors before a completion is acted on, returning a fast verdict (for example containsInjection) so applications can block or allow content.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Security
- Prompt Injection
- Threat Detection

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### PromptArmor Content Check API

Submits content (such as untrusted text an LLM is about to summarize or act on) to PromptArmor's detection engine and returns a verdict - including a containsInjection flag - indicating whether the content matches known threat classes. Authenticated with an Api-Key header.

- **Human URL:** [https://promptarmor.readme.io/reference/post_v1-check-content](https://promptarmor.readme.io/reference/post_v1-check-content)
- **Base URL:** `https://api.promptarmor.com`

#### Tags

- Security
- Prompt Injection
- Threat Detection

#### Properties

- [Documentation](https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture)
- [API Reference](https://promptarmor.readme.io/reference/post_v1-check-content)
- [OpenAPI](openapi/prompt-armor-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prompt-armor.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prompt-armor.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PromptArmor Analyze API

Analyzes LLM input (for example an email being summarized) and LLM output (for example the generated summary) through PromptArmor's default and modifiable detectors - data exfiltration, phishing, system manipulation, and adversarial instructions - to flag adversarial content in real time before a completion is acted on.

- **Human URL:** [https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture](https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture)
- **Base URL:** `https://api.promptarmor.com`

#### Tags

- Security
- Analyze
- Detectors

#### Properties

- [Documentation](https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture)
- [OpenAPI](openapi/prompt-armor-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/prompt-armor.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/prompt-armor.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PromptArmor Session Monitoring API

When a session_id is supplied on analyze requests, PromptArmor runs session-based anomaly detection, learning normal application behavior and flagging deviations across a session that may indicate a security vulnerability. Surfaced through the same analyze endpoints rather than as a standalone endpoint.

- **Human URL:** [https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture](https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture)
- **Base URL:** `https://api.promptarmor.com`

#### Tags

- Monitoring
- Anomaly Detection
- Sessions

#### Properties

- [Documentation](https://promptarmor.readme.io/reference/basics-of-promptarmor-architecture)
- [OpenAPI](openapi/prompt-armor-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/promptarmor)
- [Website](https://www.promptarmor.com/)
- [Documentation](https://promptarmor.readme.io/)
- [Plans](plans/prompt-armor-plans-pricing.yml)
- [Rate Limits](rate-limits/prompt-armor-rate-limits.yml)
- [Fin Ops](finops/prompt-armor-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
