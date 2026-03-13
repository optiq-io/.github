<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/optiq-io/.github/main/profile/logo-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/optiq-io/.github/main/profile/logo-dark.png">
    <img alt="optiq.io" src="https://raw.githubusercontent.com/optiq-io/.github/main/profile/logo-dark.png" width="128">
  </picture>
</p>

<br/>

<p align="center">
  <strong>Intelligent optimization infrastructure for the modern web</strong>
</p>

<p align="center">
  <a href="https://optiqio.com">Website</a> •
  <a href="https://optiqio.com/products">Products</a> •
  <a href="https://github.com/optiq-io/qbrix">Qbrix</a> •
  <a href="https://github.com/optiq-io/qbrix/blob/main/CLAUDE.md">Documentation</a> •
  <a href="https://optiqio.com/contact">Contact</a>
</p>

---

## What we build

**optiq.io** develops open-source infrastructure for real-time decision optimization at scale. Our systems help engineering teams run intelligent experiments, optimize user experiences, and make data-driven decisions—without the complexity.

### Qbrix

Our flagship project is **[Qbrix](https://github.com/optiq-io/qbrix)**—a distributed multi-armed bandit system designed for production workloads.

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   proxysvc  │────▶│   motorsvc  │────▶│    Redis    │
│   gateway   │     │  selection  │     │   params    │
└─────────────┘     └─────────────┘     └──────▲──────┘
       │                                       │
       │            ┌─────────────┐            │
       └───────────▶│  cortexsvc  │────────────┘
        feedback    │  training   │   batch update
                    └─────────────┘
```

**Key principles:**

- **Hot path isolation** — Selection in microseconds, learning in the background
- **Eventual consistency** — Redis-backed parameter propagation across instances
- **Horizontal scale** — Stateless selection services, single-writer training
- **Algorithm library** — Thompson Sampling, UCB, LinUCB, EXP3, and more

<br/>

## Our approach

We believe optimization infrastructure should be:

| | |
|---|---|
| **Open** | MIT licensed, community-driven, no vendor lock-in |
| **Observable** | Every decision traceable, every experiment auditable |
| **Composable** | Clean APIs, gRPC-first, plays well with your stack |
| **Production-ready** | Battle-tested patterns, Kubernetes-native deployment |

<br/>

## Get involved

We're building in the open and welcome contributions:

- Browse our [repositories](https://github.com/orgs/optiq-io/repositories)
- Read the [Qbrix architecture guide](https://github.com/optiq-io/qbrix/blob/main/CLAUDE.md)
- Open an issue or submit a PR

<br/>

---

<p align="center">
  <sub>Building the future of adaptive systems</sub>
</p>
