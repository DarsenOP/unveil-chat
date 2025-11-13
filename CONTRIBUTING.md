# Contributing to Unveil

First off, thank you for considering contributing to Unveil! It's people like you that make this open source community such a great place to learn, inspire, and create. All contributions are welcome, including bug reports, feature requests, documentation improvements, and code changes.

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Development Workflow](#development-workflow)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Bug Reports](#bug-reports)
- [Feature Requests](#feature-requests)
- [Community](#community)

## Code of Conduct

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before participating. We're committed to providing a friendly, safe, and welcoming environment for all.

## Getting Started

### Prerequisites
- **Go Backend**: Go 1.19+, PostgreSQL, Redis
- **Python AI Service**: Python 3.9+, pip, virtualenv
- **Mobile App**: Node.js 16+, React Native CLI, Android Studio/Xcode

### Quick Start
1. **Fork** the repository you want to contribute to
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/DarsenOP/unveil-chat.git
   cd unveil-chat
   ```
3. **Set up upstream**:
   ```bash
   git remote add upstream https://github.com/DarsenOP/unveil-chat.git
   ```
4. **Create a branch** for your feature:
   ```bash
   git checkout -b feature/amazing-feature
   ```

## Project Structure

We have three main repositories:

### [go-chat-backend](https://github.com/DarsenOP/unveil-chat/go-chat-backend)

- Real-time chat server and core backend
- Handles WebSocket connections, user management, matching logic
- **Primary Language**: Go

### [python-ai-service](https://github.com/DarsenOP/unveil-chat/python-ai-service)

- AI-powered conversation analysis and compatibility matching
- NLP, sentiment analysis, machine learning models
- **Primary Language**: Python

### [mobile-app](https://github.com/DarsenOP/unveil-chat/mobile-app)

- React Native mobile application for iOS and Android
- User interface, chat components, swiping functionality
- **Primary Language**: JavaScript/TypeScript

## Development Workflow

### 1. Find an Issue

- Check [Good First Issues](https://github.com/DarsenOP/unveil-chat/blob/main/.github/ISSUE_TEMPLATE/good-first-issue.md) if you're new
- Comment on the issue to let us know you're working on it
- Ask questions if anything is unclear

### 2. Make Your Changes

```bash
# Sync with main repository
git fetch upstream
git rebase upstream/main

# Make your changes and test thoroughly
# Follow our coding standards below
```

### 3. Test Your Changes

**Go Backend:**

```bash
go test ./...
go run main.go
```

**Python AI Service:**

```bash
python -m pytest
uvicorn app:app --reload
```

**Mobile App:**

```bash
npm test
npx react-native run-android  # or run-ios
```

### 4. Submit Pull Request

See [Pull Request Process](#pull-request-process) below.

## Pull Request Process

- **Ensure** all tests pass and you've added new tests for your changes
- **Update** documentation if you've changed functionality
- **Follow** our commit message conventions
- **Submit PR** with a clear title and description:
  - What changes did you make?
  - Why did you make these changes?
  - Any breaking changes?
  - Screenshots (for UI changes)

### PR Template:

```markdown
## Description
Brief description of the changes

## Related Issues
Fixes #(issue number)

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
Describe the tests you ran to verify your changes

## Screenshots (if applicable)
```

## Coding Standards

### Go Backend

- Use `gofmt` for formatting
- Follow [Effective Go](https://go.dev/doc/effective_go) guidelines
- Write unit tests with the standard `testing` package
- Use meaningful variable names, avoid abbreviations

### Python AI Service

- Follow [PEP 8](https://pep8.org/) style guide
- Use type hints where possible
- Document functions with docstrings
- Use `black` for code formatting

### Mobile App (React Native)

- Use TypeScript for type safety
- Follow React Native best practices
- Use functional components with hooks
- Use meaningful component and variable names

### General

- Write clear, readable code
- Comment complex logic, but write self-documenting code when possible
- Keep functions small and focused on single responsibility

## Commit Message Guidelines

We follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

```text
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Types:

- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code changes that neither fix bugs nor add features
- `test`: Adding or correcting tests
- `chore`: Maintenance tasks

### Examples:

```text
feat(chat): add typing indicators to chat interface

fix(auth): resolve login token expiration issue

docs(readme): update installation instructions
```

## Bug Reports

When reporting bugs, please include:

- Clear description of the issue
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Environment (OS, browser, device, app version)

Use our [bug report template](https://github.com/DarsenOP/unveil-chat/blob/main/.github/ISSUE_TEMPLATE/bug_report.md)

## Feature Requests

We love new ideas! For feature requests:

- Check if the feature already exists
- Explain the problem it solves
- Describe your proposed solution
- Provide examples or mockups if possible

Use our [feature request template](https://github.com/DarsenOP/unveil-chat/tree/main/.github/ISSUE_TEMPLATE/feature_request.md)

<!--## Community

### Get in Touch

- Discord: Join our server
- Email: team@sparkbeforesight.com
- Twitter: @SparkBeforeSight

### Recognition

All contributors get:

- Shoutouts in our release notes
- Contributor role in Discord
- Listed in our CONTRIBUTORS.md file

### Need Help?

- Ask in our Discord #help channel
- Comment on the issue you're working on
- Don't hesitate to reach out to maintainers
-->

### License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing to making anonymous connections more meaningful! 
