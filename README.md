# url-probe-smoke-test

End-to-end smoke test repository: probes the reserved documentation domain `example.com`, records the result, and validates the record with a workflow.

## Contents

- [probe-report.md](probe-report.md) — the probe result: target URL, returned title, word count, and SHA-256 checksum.
- `.github/workflows/probe.yml` — manually triggered workflow that checks the report file exists and echoes the recorded checksum.

## Usage

Run the **probe** workflow from the Actions tab to verify the report file is present and to echo its recorded checksum.
