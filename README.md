# JD Davenport

I run a production multi-agent AI organization on Claude. It sends email as me, fixes code without me watching, and operates on real money and real hardware, daily since April 2026. This account is the open half: the pieces I pulled out, cleaned up, and licensed so anyone can run them.

Everything here is bring-your-own-key and self-hostable. More at [jddavenport.com](https://jddavenport.com).

## Start with the case study

[**agent-safety-case-study**](https://github.com/jddavenportOpen/agent-safety-case-study) is the honest account of running that system: each capability paired with the risk it creates, the control that bounds it, the tradeoff I accepted, and a dated incident where the control was not enough. It includes the review panel whose 3-of-3 quorum turned out to be 1-of-3 with a hardcoded receipt, and what that cost to find.

## The six

**[orchestra-agents](https://github.com/jddavenportOpen/orchestra-agents)**
The orchestration and eval core as installable code: fan-out under bounded concurrency, a durable message bus with a strict status machine and loud dead-lettering, per-dependency circuit breakers, best-of-N with an adversarial judge, and permission tiers from READ to IRREVERSIBLE behind a human-approval gate and a hash-chained audit log. 61 offline tests. The example runs with no API key.

**[claude-deploy-kit](https://github.com/jddavenportOpen/claude-deploy-kit)**
The same discipline packaged for a real deployment: one default-deny policy chokepoint, a destructive-command deny hook that still works under skip-permissions, a fail-closed eval gate, a redacting audit log, and a secrets-provider contract. Every number in the repo is produced by the included tests.

**[mcp-judge](https://github.com/jddavenportOpen/mcp-judge)**
A calibrated LLM-as-judge exposed over MCP, shipped with the eval harness that proves the calibration. It names four judge failure modes, mid-band compression, severity bias, score-to-decision decoupling, and self-inconsistency, and fixes each one rather than asserting the scores are fine.

**[claude-bug-squash](https://github.com/jddavenportOpen/claude-bug-squash)**
Autonomous bug fixing that out of the box can never merge. Red-to-green reproduction proof, blast-radius caps checked against the actual diff, a never-touch deny list, a three-seat adversarial panel, shadow mode by default, one auto-merge per day, and an explicit arm switch.

**[recruit-copilot](https://github.com/jddavenportOpen/recruit-copilot)**
A Claude Code plugin that treats a job search as a verification problem: intake, goals, scouting, tailoring, and a calibrated grading panel with layout and round-trip gates. It does not apply for you. That is the point, not a limitation.

## Everything else

Agents and tooling: [fleetwright](https://github.com/jddavenportOpen/fleetwright) (self-hosted agent-operations OS) · [clawdling](https://github.com/jddavenportOpen/clawdling) (BYOK personal AI assistant) · [deep-research-agent](https://github.com/jddavenportOpen/deep-research-agent) (research with an adversarial verification pass) · [harnessview](https://github.com/jddavenportOpen/harnessview) (visualize a Claude Code harness and flag broken wiring) · [context-kit](https://github.com/jddavenportOpen/context-kit) (personal-context templates and skills) · [voiceclaw](https://github.com/jddavenportOpen/voiceclaw) (voice agent over the phone)

Evals and analysis: [vibe-coding-detector](https://github.com/jddavenportOpen/vibe-coding-detector) · [agi-readiness-auditor](https://github.com/jddavenportOpen/agi-readiness-auditor) · [resume-grader](https://github.com/jddavenportOpen/resume-grader) · [ai-spend-tracker](https://github.com/jddavenportOpen/ai-spend-tracker) · [mastery-engine](https://github.com/jddavenportOpen/mastery-engine)

Self-hosted tools: [openbudget](https://github.com/jddavenportOpen/openbudget) · [openplaud](https://github.com/jddavenportOpen/openplaud) · [open-remarkable](https://github.com/jddavenportOpen/open-remarkable) · [byu-outlook-browser-integration](https://github.com/jddavenportOpen/byu-outlook-browser-integration)

Teaching and product: [ai-fluency-trainer](https://github.com/jddavenportOpen/ai-fluency-trainer) · [pitchgrade](https://github.com/jddavenportOpen/pitchgrade) · [venture-val](https://github.com/jddavenportOpen/venture-val) · [caseprep](https://github.com/jddavenportOpen/caseprep) · [acquisitor](https://github.com/jddavenportOpen/acquisitor)

Licenses vary by repo. Check the LICENSE file in each one. PRs welcome.
