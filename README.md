# AI-in-Cybersecurity

Hands-on course materials for practical SOC workflows, progressing from environment setup to evidence-driven detection and then AI-assisted triage.

## Labs

1. `labs/1.0-Instance-setup.md`
	- Build and access a Linux VM from VS Code over SSH.
	- Practice Linux terminal basics and file-permission security concepts.

2. `labs/2.0-Event-Collection-and-Risk-Scoring.md`
	- Simulate controlled suspicious activity.
	- Capture and pivot Linux auth and sudo evidence.
	- Rank findings with an explainable Python risk-scoring script.

3. `labs/3.0-Wazuh-Endpoint-and-SIEM-Integration.md` (Optional)
	- Add Wazuh endpoint telemetry on Amazon Linux 2023.
	- Export endpoint alerts and forward into SIEM ingestion (Splunk HEC example).
	- Rank endpoint alerts with Python for analyst triage.

4. `labs/4.0-Bedrock-Agent-SOC-Triage.md`
	- Create a Bedrock Agent specialized for SOC triage.
	- Build and manually test Lambda-based AI triage.
	- Add IAM guardrails and structured response validation.

5. `labs/5.0-Event-Driven-Bedrock-SOC-Automation.md`
	- Trigger AI triage automatically from new Wazuh alert files in S3.
	- Store structured triage artifacts for analyst review.
	- Prepare the workflow for SIEM write-back or later automation.

## Suggested Learning Flow

1. Foundation: environment + Linux fundamentals.
2. Detection basics: event generation, evidence capture, and rule-based scoring.
3. Optional endpoint telemetry: Wazuh agent alerts + SIEM forwarding.
4. AI augmentation: manual Bedrock triage with guardrails and validation.
5. Automation: event-driven Bedrock triage pipeline.