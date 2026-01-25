# Contributing to Spinning Board Game

Thank you for your interest in contributing to Spinning Board Game! This document provides guidelines and instructions for contributing.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Setup](#development-setup)
- [Making Contributions](#making-contributions)
- [Pull Request Process](#pull-request-process)
- [Code Style Guidelines](#code-style-guidelines)
- [Testing](#testing)
- [Reporting Bugs](#reporting-bugs)
- [Feature Requests](#feature-requests)

## 📜 Code of Conduct

Please be respectful and inclusive in all interactions. We welcome contributors of all backgrounds and experience levels.

## 🚀 Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/SpinningB.git
   cd SpinningB
   ```
3. **Add upstream remote**:
   ```bash
   git remote add upstream https://github.com/phessophissy/SpinningB.git
   ```

## 🛠️ Development Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher)
- [Clarinet](https://github.com/hirosystems/clarinet) (for smart contract development)
- A code editor (VS Code recommended)
- Git

### Installation

1. Install Node.js dependencies:
   ```bash
   npm install
   ```

2. Install Clarinet (for smart contract work):
   ```bash
   # macOS
   brew install clarinet

   # Windows (using winget)
   winget install hirosystems.clarinet

   # Linux
   curl -L https://github.com/hirosystems/clarinet/releases/download/v2.3.0/clarinet-linux-x64.tar.gz | tar xz
   sudo mv clarinet /usr/local/bin/
   ```

3. Run the frontend locally:
   ```bash
   cd frontend && python3 -m http.server 8080
   # Or
   npx http-server frontend -p 8080
   ```

4. Open http://localhost:8080 in your browser

## 💡 Making Contributions

### Types of Contributions Welcome

- 🐛 Bug fixes
- ✨ New features
- 📚 Documentation improvements
- 🎨 UI/UX enhancements
- 🧪 Tests
- 🔧 Code refactoring

### Before You Start

1. Check the [Issues](https://github.com/phessophissy/SpinningB/issues) page for existing discussions
2. For major changes, open an issue first to discuss your proposal
3. Make sure your contribution aligns with the project's goals

## 🔄 Pull Request Process

1. **Create a feature branch**:
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

2. **Make your changes** and commit with clear messages:
   ```bash
   git add .
   git commit -m "feat: add new feature description"
   # or
   git commit -m "fix: resolve issue with X"
   ```

3. **Keep your fork updated**:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```

4. **Push to your fork**:
   ```bash
   git push origin feature/your-feature-name
   ```

5. **Open a Pull Request** on GitHub with:
   - Clear title describing the change
   - Description of what was changed and why
   - Reference to any related issues (e.g., "Fixes #123")
   - Screenshots for UI changes

### Commit Message Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):

| Type | Description |
|------|-------------|
| `feat` | New feature |
| `fix` | Bug fix |
| `docs` | Documentation only |
| `style` | Formatting, no code change |
| `refactor` | Code restructuring |
| `test` | Adding tests |
| `chore` | Maintenance tasks |

Examples:
- `feat: add leaderboard feature`
- `fix: resolve wallet connection issue on mobile`
- `docs: update README with testnet instructions`

## 📝 Code Style Guidelines

### JavaScript

- Use ES6+ syntax
- Use meaningful variable and function names
- Add comments for complex logic
- Keep functions small and focused
- Use `const` and `let` (avoid `var`)

### Clarity (Smart Contracts)

- Use descriptive function and variable names
- Add comments explaining complex logic
- Follow the existing code structure
- Test thoroughly before submitting

### CSS

- Use CSS custom properties (variables) for colors
- Follow the existing naming conventions
- Keep styles modular and organized
- Ensure mobile responsiveness

### HTML

- Use semantic HTML elements
- Ensure accessibility (ARIA labels, alt text)
- Keep markup clean and well-indented

## 🧪 Testing

### Smart Contract Testing

Use Clarinet to run contract tests:

```bash
cd contracts
clarinet test
```

### Frontend Testing

Currently, we use manual testing. Contributions to add automated testing are welcome!

Before submitting a PR, please verify:
- [ ] The app loads without errors
- [ ] Wallet connection works
- [ ] Game mechanics function correctly
- [ ] UI displays properly on desktop and mobile

## 🐛 Reporting Bugs

When reporting bugs, please include:

1. **Description**: Clear description of the bug
2. **Steps to Reproduce**: Numbered steps to reproduce the issue
3. **Expected Behavior**: What should happen
4. **Actual Behavior**: What actually happens
5. **Environment**: Browser, OS, wallet used
6. **Screenshots**: If applicable

Use the [Issues](https://github.com/phessophissy/SpinningB/issues) page with the "bug" label.

## ✨ Feature Requests

For feature requests, please include:

1. **Problem Statement**: What problem does this solve?
2. **Proposed Solution**: How should it work?
3. **Alternatives Considered**: Other approaches you've thought about
4. **Additional Context**: Mockups, examples, etc.

Use the [Issues](https://github.com/phessophissy/SpinningB/issues) page with the "enhancement" label.

## 📬 Questions?

If you have questions, feel free to:
- Open an issue with the "question" label
- Check existing issues for similar questions

---

Thank you for contributing! 🎰🌊
