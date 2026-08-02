# Callisto Media

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
