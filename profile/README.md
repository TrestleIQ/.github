<br>

<p align="center">
  <a target="_blank" rel="noopener noreferrer" href="https://trestleiq.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/TrestleIQ/.github/main/assets/trestle-logo-white.webp">
      <img alt="Trestle" src="https://raw.githubusercontent.com/TrestleIQ/.github/main/assets/trestle-logo.webp" width="220">
    </picture>
  </a>
</p>

<p align="center">
  <strong>Identity data APIs for sales, contact centers, and trust&nbsp;&amp;&nbsp;safety.</strong><br>
  <sub>Validate, verify, and enrich consumer contact information at the speed of a single API call.</sub>
</p>

<p align="center">
  <a target="_blank" rel="noopener noreferrer" href="https://portal.trestleiq.com/signup">Get an API key</a>
  &nbsp;·&nbsp;
  <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/guides/overview">Documentation</a>
  &nbsp;·&nbsp;
  <a target="_blank" rel="noopener noreferrer" href="https://status.trestleiq.com">Status</a>
  &nbsp;·&nbsp;
  <a target="_blank" rel="noopener noreferrer" href="https://trestleiq.com">trestleiq.com</a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/TrestleIQ/.github/main/assets/brand-bar.svg" alt="" width="100%" height="6">
</p>

<br>

## Products

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3>Real Contact API</h3>
      <p>Score and verify a lead's phone, email, and postal address in a single call — built for inbound forms and lead routing.</p>
      <p><code>GET /2.0/real_contact</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/real-contact-api">Reference&nbsp;→</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Caller Identification API</h3>
      <p>Identify the person behind an inbound number in real time, with line type and location for smarter routing.</p>
      <p><code>GET /3.1/caller_id</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/caller-identification-api">Reference&nbsp;→</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Smart CNAM API</h3>
      <p>Lightweight caller name lookup. Returns just the name on the line — optimized for high-volume call display and screening.</p>
      <p><code>GET /3.1/cnam</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/smart-cnam-api">Reference&nbsp;→</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Phone Validation API</h3>
      <p>Confirm a number is active and dialable, with line type, carrier, country, and prepaid status. Global coverage.</p>
      <p><code>GET /3.0/phone_intel</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/phone-validation-api">Reference&nbsp;→</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Reverse Phone API</h3>
      <p>Every person and address historically linked to a phone number — for skip tracing, fraud, and enrichment workflows.</p>
      <p><code>GET /3.2/phone</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/reverse-phone-api">Reference&nbsp;→</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Reverse Address API</h3>
      <p>Current and prior US residents at a street address, with linked phones and demographics.</p>
      <p><code>GET /3.1/location</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/reverse-address-api">Reference&nbsp;→</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Phone Feedback API</h3>
      <p>Send live-call outcomes back to Trestle so future lookups reflect what you learned. Closes the loop on data quality.</p>
      <p><code>POST /1.0/phone_feedback</code> &nbsp;·&nbsp; <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/api-reference/phone-feedback-api">Reference&nbsp;→</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Ready to build?</h3>
      <p>Sign up for a key, drop your first request, and you're live in under five minutes.</p>
      <p><a target="_blank" rel="noopener noreferrer" href="https://portal.trestleiq.com/signup"><strong>portal.trestleiq.com&nbsp;→</strong></a></p>
    </td>
  </tr>
</table>

<br>

## Quickstart

```bash
curl "https://api.trestleiq.com/3.0/phone_intel?phone=2069735100" \
  -H "x-api-key: $TRESTLE_API_KEY"
```

Every endpoint shares one base URL (`https://api.trestleiq.com`) and one header (`x-api-key`). See the <a target="_blank" rel="noopener noreferrer" href="https://docs.trestleiq.com/guides/authentication">authentication guide</a> for key management.

<br>

## Why teams choose Trestle

<table width="100%">
  <tr>
    <td width="33%" align="center" valign="top">
      <h4>Built for production</h4>
      <sub>99.95% uptime SLA. Sub-second median responses. SOC 2 Type I certified.</sub>
    </td>
    <td width="33%" align="center" valign="top">
      <h4>Depth of coverage</h4>
      <sub>Comprehensive US identity graph. Global phone validation and reverse phone.</sub>
    </td>
    <td width="33%" align="center" valign="top">
      <h4>Developer-first</h4>
      <sub>One header, one base URL, predictable JSON. No SDK required, no contracts to start.</sub>
    </td>
  </tr>
</table>

<br>

<p align="center">
  <img src="https://raw.githubusercontent.com/TrestleIQ/.github/main/assets/brand-bar.svg" alt="" width="100%" height="6">
</p>

<p align="center">
  <sub>
    Trestle Solutions Inc. · Bellevue, WA<br>
    Trestle data is intended for marketing, sales, contact-center, and trust-and-safety use cases<br>and is not permissible for FCRA-regulated decisions (credit, insurance, employment, housing, benefits).
  </sub>
</p>
