# Trestle Public Workspace

Welcome to the official Trestle developer workspace. Trestle provides identity data APIs that help businesses **validate**, **verify**, and **enrich** consumer contact information — turning partial leads and inbound calls into trusted, actionable identities.

This workspace is the home for every public Trestle API. Whether you're prioritizing leads, identifying inbound callers, optimizing AI voice agents, or cleaning up a CRM, you can prototype against the Trestle API in minutes.

> **Base URL:** `https://api.trestleiq.com`
> **Auth:** `x-api-key` header on every request
> **Get an API key:** [portal.trestleiq.com/signup](https://portal.trestleiq.com/signup)

---

## About Trestle

Trestle Solutions Inc. is a B2B identity data company headquartered in Bellevue, WA. We maintain one of the most comprehensive contact graphs in the United States — names, phones, addresses, and emails — refreshed continuously from authoritative sources.

- **SOC 2 Type I certified** — enterprise-grade security and data handling
- **Comprehensive US coverage** for identity enrichment and verification
- **Global coverage** for phone validation and reverse phone lookups
- **99.95% uptime SLA** across all production APIs
- **Sub-second response times** on the median request

Trestle data is engineered for marketing, sales, contact center, and trust-and-safety use cases. It is **not** permissible for FCRA-regulated decisions (credit, insurance, employment, housing, or government benefits).

---

## APIs

Each API is documented with parameters, response schemas, and live examples on [docs.trestleiq.com](https://docs.trestleiq.com).

| API | Version | Method | Endpoint | Reference |
|---|---|---|---|---|
| **Real Contact API** | v2.0 | `GET` | `/2.0/real_contact` | [docs](https://docs.trestleiq.com/api-reference/real-contact-api) |
| **Caller Identification API** | v3.1 | `GET` | `/3.1/caller_id` | [docs](https://docs.trestleiq.com/api-reference/caller-identification-api) |
| **Smart CNAM API** | v3.1 | `GET` | `/3.1/cnam` | [docs](https://docs.trestleiq.com/api-reference/smart-cnam-api) |
| **Phone Validation API** | v3.0 | `GET` | `/3.0/phone_intel` | [docs](https://docs.trestleiq.com/api-reference/phone-validation-api) |
| **Reverse Phone API** | v3.2 | `GET` | `/3.2/phone` | [docs](https://docs.trestleiq.com/api-reference/reverse-phone-api) |
| **Reverse Address API** | v3.1 | `GET` | `/3.1/location` | [docs](https://docs.trestleiq.com/api-reference/reverse-address-api) |
| **Phone Feedback API** | v1.0 | `POST` | `/1.0/phone_feedback` | [docs](https://docs.trestleiq.com/api-reference/phone-feedback-api) |

### What each API does

- **[Real Contact API](https://docs.trestleiq.com/api-reference/real-contact-api)** — score a lead in a single call. Validates phone, email, and postal address on a record and confirms whether they belong to the named contact. Ideal for lead routing, signup risk checks, and form submissions.
- **[Caller Identification API](https://docs.trestleiq.com/api-reference/caller-identification-api)** — returns the most likely identity behind an inbound phone number (name, age range, location, line type) so you can greet, route, and personalize calls in real time.
- **[Smart CNAM API](https://docs.trestleiq.com/api-reference/smart-cnam-api)** — lightweight caller name lookup. Returns just the name on the line, optimized for high-volume call display and screening flows.
- **[Phone Validation API](https://docs.trestleiq.com/api-reference/phone-validation-api)** — confirms a phone number is active and dialable, with line type, carrier, country, and prepaid status. Use it before outbound dialing or texting to suppress disconnects and reduce TCPA risk.
- **[Reverse Phone API](https://docs.trestleiq.com/api-reference/reverse-phone-api)** — returns every person and address historically associated with a phone number. Powers skip tracing, debt recovery, fraud investigation, and contact-data enrichment workflows.
- **[Reverse Address API](https://docs.trestleiq.com/api-reference/reverse-address-api)** — returns current and prior residents at a U.S. street address, with linked phones and demographics. Useful for address verification, household enrichment, and door-to-door routing.
- **[Phone Feedback API](https://docs.trestleiq.com/api-reference/phone-feedback-api)** — submit live-call outcomes (answered, disconnected, wrong-party, do-not-call) back to Trestle so future lookups reflect what you learned. Closes the loop between dialing and data quality.

---

## Quickstart

### 1. Get an API key
[Sign up at portal.trestleiq.com](https://portal.trestleiq.com/signup). After verification, your key is available in the portal dashboard.

### 2. Send your first request

```bash
curl --request GET \
  --url "https://api.trestleiq.com/3.0/phone_intel?phone=2069735100" \
  --header "x-api-key: YOUR_API_KEY"
```

### 3. Pick the right API for your use case

| Goal | Use this API |
|---|---|
| Verify a lead's phone, email, and address quality | Real Contact API |
| Look up everyone associated with a phone number | Reverse Phone API |
| Identify an inbound caller in real time | Caller Identification API |
| Get just a caller's display name | Smart CNAM API |
| Validate a phone and get carrier / line type | Phone Validation API |
| Look up residents at a street address | Reverse Address API |
| Send live-call outcomes back to Trestle | Phone Feedback API |

For authentication details, see the [authentication guide](https://docs.trestleiq.com/guides/authentication).

---

## Popular use cases

- **Lead qualification & routing** — score and prioritize inbound web leads
- **Contact data enrichment** — turn a phone or email into a complete profile
- **AI voice agent optimization** — give voice agents richer caller context
- **Inbound call routing & personalization** — greet callers by name, route by intent
- **Outbound contact rate improvement** — suppress bad numbers before dialing
- **Signup & onboarding risk reduction** — flag risky form submissions in-line
- **CRM hygiene** — clean phones, emails, and addresses at scale
- **Fraud detection** — cross-check identities against the Trestle graph
- **TCPA compliance support** — confirm line type and reassignment status

---

## Resources

- **Documentation:** [docs.trestleiq.com](https://docs.trestleiq.com/guides/overview)
- **Developer Portal:** [portal.trestleiq.com](https://portal.trestleiq.com)
- **Status page:** [status.trestleiq.com](https://status.trestleiq.com)
- **Company website:** [trestleiq.com](https://trestleiq.com)

## Support

- **API & integration questions:** [support@trestleiq.com](mailto:support@trestleiq.com)
- **Incident updates:** subscribe at [status.trestleiq.com](https://status.trestleiq.com)

---

*© Trestle Solutions Inc. — Bellevue, WA. Trestle data is intended for marketing, sales, contact-center, and trust-and-safety uses, and is not permissible for FCRA-regulated decisions.*
