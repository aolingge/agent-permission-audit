<p align="center">
  <img src="assets/readme-banner.svg" alt="Agent Permission Audit banner" width="100%">
</p>

<h1 align="center">Agent Permission Audit</h1>

<p align="center">Audit repo docs for risky AI agent permissions around files, shell, browser, network, and secrets.</p>

<p align="center"><a href="README.zh-CN.md">中文</a> · <a href="#quick-start">Quick Start</a> · <a href="#checks">Checks</a></p>

<p align="center">
  <img alt="Node.js" src="https://img.shields.io/badge/node-%3E%3D18-2563EB">
  <img alt="dependencies" src="https://img.shields.io/badge/dependencies-0-111827">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-16A34A">
</p>

<p align="center">
  <img src="assets/cli-preview.svg" alt="Agent Permission Audit CLI preview" width="88%">
</p>

## Why This Exists

AI agent workflows keep growing, but many repos still lack tiny local checks that are easy to run in CI. This tool stays zero-dependency, mirror-friendly, and easy to fork.

## Quick Start

```bash
npx github:aolingge/agent-permission-audit --path AGENTS.md
```

Generate Markdown:

```bash
npx github:aolingge/agent-permission-audit --path AGENTS.md --markdown > report.md
```

Generate SARIF:

```bash
npx github:aolingge/agent-permission-audit --path AGENTS.md --sarif > results.sarif
```

## Checks

| Check | What it looks for |
| --- | --- |
| filesystem | Mentions file access. |
| shell | Mentions shell command rules. |
| network | Mentions network or browser access. |
| secrets | Mentions secret boundary. |

## CI Usage

See [docs/github-actions.md](docs/github-actions.md).

## Mirrors

- GitHub: https://github.com/aolingge/agent-permission-audit
- Gitee: https://gitee.com/aolingge/agent-permission-audit

## Visual Identity

The banner and CLI preview are SVG assets committed in `assets/`, so the README renders cleanly on GitHub and Gitee without external image hosting.

## Contributing

Good first PRs: add checks, add fixtures, improve docs, or add GitHub Actions examples.

## License

MIT
