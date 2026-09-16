# WS03 Free Windows Runner

Generic, public canary harness for WS03 Remote Compute.

This repository intentionally contains **no private WS03 source, credentials, user payloads, or private artifacts**. It exists only to prove properties of GitHub-hosted ephemeral Windows runners that are free for public repositories.

The workflow is manual-only, uses a standard `windows-2025` runner, has a 10-minute hard timeout, installs Microsoft's WinApp CLI from a commit-pinned setup action, creates a synthetic local WinForms target, verifies UI Automation plus screenshot capture, probes real input injection separately, prints secret-free evidence, and uploads nothing.

The public runner is not automatically equivalent to the stronger WS03 `windows_gui` contract. Any capability not demonstrated by the canary remains fail-closed.
