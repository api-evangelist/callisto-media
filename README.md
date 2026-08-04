# Callisto Media

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

Callisto Media Inc. was a data-driven nonfiction book publisher founded in 2011 by CEO Benjamin Wayne,
with offices in Oakland (earlier Emeryville), California and New York. It commissioned instructional
titles from demand signals — point-of-sale data, search volume and category gaps — rather than editorial
instinct, publishing chiefly through the **Rockridge Press** imprint and the **Callisto Kids** line.
Its publishing assets were acquired by **Sourcebooks** on 9 May 2023 in a deal funded by Penguin Random
House, and the brand now trades as **Callisto Publishing**, a Sourcebooks imprint.

## API surface

**None.** Enrichment probes on 2026-08-02 found no machine-readable contract of any kind:

- `callistomedia.com` does not answer on port 443; HTTP/80 returns `301` to `callistopublishing.com`,
  which `301`s again to `https://www.sourcebooks.com/callisto/`.
- `/openapi.json`, `/swagger.json` and `/.well-known/ai-plugin.json` → `404` on every host.
- `/.well-known/agent-card.json` and `/.well-known/agent.json` → `404` on every host (no A2A agent card).
- Other probed paths return `200` with the Sourcebooks Magento single-page-application HTML shell —
  a catch-all response, not a document.
- No developer portal, no GitHub organization, no SDK on npm or PyPI, no `llms.txt`.

## Artifacts

| Path | Type | Method |
|---|---|---|
| `well-known/callisto-media-well-known.yml` | WellKnown | probed |
| `security/callisto-media-domain-security.yml` | DomainSecurity | probed |
| `llms/callisto-media-llms.txt` | LLMsTxt | generated |

## Links

- Callisto brand page: https://www.sourcebooks.com/callisto/
- Archived company site (March 2023): https://web.archive.org/web/20230316111229/https://www.callistomedia.com/
- Acquisition announcement: https://www.prnewswire.com/news-releases/callisto-media-to-join-leading-independent-publisher-sourcebooks-301820039.html
- Secondary-market listing: https://forgeglobal.com/callisto-media_stock/
