# Continum Documentation

Official documentation for Continum - the distributed compliance layer for LLMs.

## What's Included

This documentation covers:

- **Getting Started**: Quick installation and setup guides
- **Core Concepts**: Architecture, zero-latency auditing, Guardian, Mirror, Sandbox, Signal
- **SDK Integration**: TypeScript/JavaScript SDK with OpenAI, Anthropic, and Gemini support
- **Compliance**: PII detection, bias detection, security auditing, and more
- **API Reference**: Complete REST API documentation
- **Dashboard**: Using the web console for monitoring

## Documentation Structure

```
apps/docs/
├── index.mdx                    # Homepage
├── quickstart.mdx               # 5-minute quickstart
├── concepts/                    # Core concepts
│   ├── architecture.mdx
│   ├── zero-latency.mdx
│   ├── guardian.mdx
│   ├── mirror.mdx
│   ├── sandbox.mdx
│   └── signal.mdx
├── sdk/                         # SDK documentation
│   ├── installation.mdx
│   ├── configuration.mdx
│   ├── openai.mdx
│   ├── anthropic.mdx
│   ├── gemini.mdx
│   ├── streaming.mdx
│   ├── vision.mdx
│   └── tools.mdx
├── compliance/                  # Compliance guides
│   ├── pii-detection.mdx
│   ├── bias-detection.mdx
│   ├── security-audit.mdx
│   ├── prompt-injection.mdx
│   ├── agent-safety.mdx
│   ├── hallucination.mdx
│   └── regulations.mdx
├── dashboard/                   # Dashboard guides
│   ├── overview.mdx
│   ├── signals.mdx
│   ├── sandboxes.mdx
│   └── api-keys.mdx
└── api-reference/              # API documentation
    ├── introduction.mdx
    ├── authentication.mdx
    ├── customer/
    ├── sandbox/
    ├── guardian/
    ├── mirror/
    └── dashboard/
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

### Zero-Latency Auditing
- How Continum achieves 0ms added latency
- Direct LLM execution with async compliance
- Guardian pre-LLM protection (< 100ms)

### Comprehensive Detection
- 15+ sandbox types for different compliance needs
- PII, bias, security, prompt injection, agent safety
- Hallucination, financial/legal compliance

### Privacy-First Architecture
- API keys stay on your server
- Only compliance triplets sent to Continum
- Stateless sandbox isolation

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
