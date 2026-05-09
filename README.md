# AgentAudit — AI Agent Security Scanner

> Automated security scanner for AI agents. Detect prompt injection, PII leakage, unauthorized tool use, and SSRF attacks — before they hit production.

![AgentAudit Terminal Demo](https://img.shields.io/badge/scan%20time-%3C60s-brightgreen)
![Open Source](https://img.shields.io/badge/license-MIT-blue)
![Version](https://img.shields.io/badge/version-1.0%20Beta-orange)

## Why AgentAudit?

AI agents are a security blind spot. Traditional security tools don't understand agent behavior, and attackers know this.

- **Prompt Injection**: Malicious inputs hijack your agent's behavior
- **PII Leakage**: Agents inadvertently expose customer data
- **Tool Misuse**: Overprivileged access enables destructive operations
- **SSRF Attacks**: Agents fetching URLs can access internal services

## Features

| Feature | Open Source | Pro ($29/mo) | Team ($79/mo) |
|---------|:-----------:|:------------:|:-------------:|
| Static Analysis | ✅ | ✅ | ✅ |
| Prompt Injection Detection | ✅ | ✅ | ✅ |
| PII Scanning | ✅ | ✅ | ✅ |
| CLI Tool | ✅ | ✅ | ✅ |
| Dynamic Fuzzing | ❌ | ✅ | ✅ |
| Tool Permission Audit | ❌ | ✅ | ✅ |
| GitHub Action | ❌ | ✅ | ✅ |
| Security Dashboard | ❌ | ❌ | ✅ |
| SSO / SAML | ❌ | ❌ | ✅ |
| Team Members | 1 | 5 | Unlimited |

## Quick Start

```bash
# Install
npm i -g agentaudit

# Scan your agent
agentaudit scan --agent my-agent.yaml

# Auto-fix issues
agentaudit fix --agent my-agent.yaml

# CI/CD integration
agentaudit scan --fail-on high
```

## GitHub Action

```yaml
- name: Security Scan
  uses: crazycompanyinc/agentaudit-action@v1
  with:
    agent-config: ./agent.yaml
    fail-on: high
```

## Supported Frameworks

- ✅ LangChain
- ✅ CrewAI
- ✅ AutoGen
- ✅ OpenAI Agents SDK
- ✅ Custom agents (any config format)
- ✅ MCP-compatible tools

## Pricing

| Plan | Price | Best For |
|------|-------|----------|
| Open Source | $0 | Individual developers |
| Pro | $29/mo | Teams in production |
| Team | $79/mo | Multiple agent teams |

## Comparison

| Feature | AgentAudit | Pangea | Pipelock | Manual |
|---------|:----------:|:------:|:--------:|:------:|
| Open Source Core | ✅ | ❌ | ✅ | ❌ |
| Self-Hosted | ✅ | ❌ | ✅ | ✅ |
| Free Tier | ✅ | ❌ | ✅ | ✅ |
| Tool Permission Audit | ✅ | ❌ | ❌ | ❌ |
| CI/CD Integration | ✅ | ✅ | ✅ | ❌ |

## Roadmap

- [x] Static analysis engine
- [x] Prompt injection detection
- [x] PII scanning
- [ ] Dynamic fuzzing (Pro)
- [ ] MCP security audit
- [ ] Team dashboard
- [ ] Slack/Discord alerts

## Contributing

We welcome contributions! See [CONTRIBUTING.md](./CONTRIBUTING.md) for details.

## License

MIT © 2026 [ZOO](https://zoo.dev)
