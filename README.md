# PromptArmor (prompt-armor)

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
