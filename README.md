# Continum Documentation

Official documentation for Continum - the compliance infrastructure for AI applications.

## What's Included

This documentation covers:

- **Getting Started**: Quick installation and setup guides
- **Core Concepts**: Architecture, zero-latency monitoring, Guardian, Sandbox, Signal, Evidence, Incidents
- **SDK Integration**: TypeScript/JavaScript SDK with OpenAI, Anthropic, and Gemini support
- **Compliance**: Evidence generation, regulatory frameworks (GDPR, SOC 2, ISO 27001, HIPAA, etc.)
- **API Reference**: Complete REST API documentation including Evidence API
- **Dashboard**: Using the web console for monitoring and evidence management
- **CLI**: Command-line interface for team deployment

## Documentation Structure

```
apps/docs/
├── index.mdx                    # Homepage
├── quickstart.mdx               # 5-minute quickstart
├── concepts/                    # Core concepts
│   ├── architecture.mdx         # System architecture
│   ├── zero-latency.mdx         # Zero-latency monitoring
│   ├── guardian.mdx             # Pre-LLM protection
│   ├── mirror.mdx               # Async monitoring
│   ├── sandbox.mdx              # Monitoring configuration
│   ├── signal.mdx               # Compliance signals
│   ├── evidence.mdx             # Compliance evidence
│   └── incidents.mdx            # Incident management
├── compliance/                  # Compliance guides
│   └── regulations.mdx          # Regulatory frameworks
├── sdk/                         # SDK documentation
│   ├── installation.mdx
│   ├── configuration.mdx
│   ├── openai.mdx
│   ├── anthropic.mdx
│   ├── gemini.mdx
│   ├── streaming.mdx
│   ├── vision.mdx
│   └── models.mdx
├── cli/                         # CLI documentation
│   ├── overview.mdx
│   ├── installation.mdx
│   ├── authentication.mdx
│   ├── commands.mdx
│   ├── configuration.mdx
│   └── team-deployment.mdx
├── dashboard/                   # Dashboard guides
│   ├── overview.mdx
│   ├── signals.mdx
│   ├── sandboxes.mdx
│   ├── api-keys.mdx
│   └── evidence.mdx
└── api-reference/              # API documentation
    ├── introduction.mdx
    ├── authentication.mdx
    └── evidence-introduction.mdx
```

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview documentation locally:

```bash
npm i -g mint
```

Run the development server:

```bash
cd apps/docs
mint dev
```

View your local preview at `http://localhost:3000`.

## Key Features Documented

### Zero-Latency Monitoring
- How Continum achieves 0ms added latency
- Direct LLM execution with async compliance
- Guardian pre-LLM protection (< 100ms)

### Comprehensive Detection
- 15+ sandbox types for different compliance needs
- PII, bias, security, prompt injection, agent safety
- Hallucination, financial/legal compliance

### Compliance Evidence
- Cryptographic hash chain integrity
- Regulatory attestations (GDPR, SOC 2, ISO 27001, HIPAA, etc.)
- Incident management with segregation of duties
- Audit-ready evidence packages

### Privacy-First Architecture
- API keys stay on your server
- Only compliance signals sent to Continum
- Encrypted storage and transmission
- Role-based access controls

### Real-Time Monitoring
- Dashboard for viewing signals
- Risk level breakdown
- Filter by sandbox, provider, model, date

## Publishing Changes

Documentation is automatically deployed when changes are pushed to the main branch.

## Need Help?

- **Documentation**: [docs.continum.co](https://docs.continum.co)
- **Dashboard**: [console.continum.co](https://console.continum.co)
- **Support**: [support@continum.co](mailto:support@continum.co)

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on contributing to the documentation.
