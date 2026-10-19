# url-probe-smoke-test

End-to-end smoke test repository: probes the reserved documentation domain `example.com`, records the result, and validates the record with a workflow.

## Contents

- [probe-report.md](probe-report.md) — the probe result: target URL, returned title, word count, and SHA-256 checksum.
- `.github/workflows/probe.yml` — manually triggered workflow that checks the report file exists and echoes the recorded checksum.

## Latest probe

- **Title returned:** Example Domain
- **Word count:** 134
- **SHA-256 checksum:** `766c791b…`

## Usage

Run the **probe** workflow from the Actions tab to verify the report file is present and to echo its recorded checksum.
