# 🤝 Contributing to Prime Directive Labs

Thank you for your interest in contributing to Prime Directive Labs! We're building the coordination infrastructure for civilization-scale challenges, and we welcome contributions from builders who share our vision.

## 🌟 Ways to Contribute

### Code Contributions
- **Bug fixes** — Help us squash bugs across any repository
- **Features** — Implement new functionality aligned with our roadmap
- **Documentation** — Improve docs, add examples, fix typos
- **Testing** — Write tests, improve coverage, report issues

### Non-Code Contributions
- **Issue triage** — Help organize and categorize issues
- **Design** — UI/UX improvements, design system contributions
- **Community** — Help answer questions, welcome newcomers
- **Translations** — Help internationalize our content

## 🚀 Getting Started

### 1. Fork & Clone

```bash
# Clone the workspace
git clone git@github.com:Prime-Directive-Labs/primedir-workspace.git
cd primedir-workspace

# Clone all repositories
./scripts/clone-all.sh

# Open in Cursor/VSCode
cursor primedir.code-workspace
```

### 2. Start Development Environment

```bash
docker-compose up -d

# Access points:
# 🚀 Dashboard: http://localhost:3002
# 🌐 Website:   http://localhost:3003
# ⚙️ API:       http://localhost:8000
```

### 3. Create a Branch

Always work on a feature branch, never directly on `main`:

```bash
# Use descriptive names with prefixes
git checkout -b feature/add-staking-rewards
git checkout -b fix/wallet-connection-error
git checkout -b docs/update-api-reference
```

### 4. Make Your Changes

- Follow our [Code Standards](https://docs.primedir.ai/development/code-standards)
- Write tests for new functionality
- Update documentation as needed
- Ensure all tests pass

### 5. Commit Your Changes

We follow conventional commits:

```bash
git commit -m "feat(staking): add reward distribution logic

## Summary
Implemented automatic reward distribution for staked AET tokens.

## Changes
- Added RewardDistributor contract
- Integrated with GuardVault
- Added unit tests for edge cases"
```

### 6. Submit a Pull Request

- Push your branch and open a PR
- Fill out the PR template completely
- Link any related issues
- Request review from maintainers

## 📋 Commit Message Format

```
type(scope): brief description

## Summary
Detailed explanation of what and why

## Changes
- Specific change 1
- Specific change 2
```

### Types
- `feat` — New feature
- `fix` — Bug fix
- `docs` — Documentation
- `style` — Formatting (no logic change)
- `refactor` — Code restructuring
- `test` — Adding tests
- `chore` — Maintenance

## 🏗️ Repository Structure

| Repository | Focus | Stack |
|------------|-------|-------|
| `primedir-app` | Dashboard UI | Next.js, React, Wagmi |
| `primedir-web` | Marketing site | Next.js, TailwindCSS |
| `primedir-api` | Backend API | Django, DRF |
| `primedir-contracts` | Smart contracts | Solidity, Foundry |
| `primedir-docs` | Documentation | Docusaurus |

## ✅ Pull Request Checklist

- [ ] Code follows our style guidelines
- [ ] Tests added/updated as needed
- [ ] Documentation updated
- [ ] Commit messages follow convention
- [ ] No console errors or warnings
- [ ] Branch is up to date with `main`

## 🔍 Code Review

All PRs require at least one approval. Reviewers will check:

- **Functionality** — Does it work as intended?
- **Code quality** — Is it clean, readable, maintainable?
- **Testing** — Are there adequate tests?
- **Security** — Any potential vulnerabilities?
- **Performance** — Any performance concerns?

## 🎨 Style Guidelines

### TypeScript/JavaScript
- Use TypeScript strict mode
- Prettier for formatting
- ESLint for linting

### Python
- Black for formatting (line length 88)
- isort for imports
- Type hints required

### Solidity
- Follow our [Solidity Standards](https://docs.primedir.ai/contracts/style-guide)
- NatSpec documentation required
- Gas optimization where appropriate

## 💬 Getting Help

- **Discord** — [Join our community](https://discord.gg/primedir)
- **Issues** — Open an issue for bugs or questions
- **Discussions** — Use GitHub Discussions for broader topics

## 📜 License

By contributing, you agree that your contributions will be licensed under the same license as the repository you're contributing to.

---

*"We engineer civilization, not just code."*

**Prime Directive Labs** 🛡️
