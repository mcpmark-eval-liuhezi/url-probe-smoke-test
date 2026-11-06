# url-probe-smoke-test

End-to-end smoke test repository: probes the reserved documentation domain `example.com`, records the result, and validates the record with a workflow.

## Contents

- [probe-report.md](probe-report.md) — the probe result: target URL, returned title, word count, and SHA-256 checksum.
- `.github/workflows/probe.yml` — manually triggered workflow that checks the report file exists and echoes the recorded checksum.

## Latest probe

- **Title returned:** Example Domain
- **Word count:** 25
- **SHA-256 checksum:** `0a080719…`

## Usage

Run the **probe** workflow from the Actions tab to verify the report file is present and to echo its recorded checksum.

## This run

- Probed URL: `https://example.com/`
- Title returned: **Example Domain**
- Recorded word count: **25** (whitespace tokens over the page body prose)
- Recorded SHA-256: `0a080719be9fbb82a86a45b80dc8c2a430fbe17dc93d23758debac092864d00f`

These values were computed from the page content retrieved during this run (2026-11-06): the title came from the fetched markdown, the word count from whitespace-token counting of that body text, and the checksum from SHA-256 of the normalized UTF-8 content.
