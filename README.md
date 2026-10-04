# coeus-heartbeat
COEUS-down alarm. COEUS's conveyor runner (C:\HomeOps\services\conveyor\runner\conveyor-runner.ps1) sets the repo
variable HEARTBEAT every ~15 min; `.github/workflows/watch.yml` runs every 30 min on GitHub and opens an issue
assigned to shamp-cpu when the heartbeat is older than 45 min, and closes it when COEUS is back.
Approved by Sean 2026-10-03 (status\DECISIONS.md).
