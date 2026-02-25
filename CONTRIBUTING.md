# Contributing to PowerApps Components

Thank you for your interest in contributing to the PowerApps Components Library! We appreciate your efforts to make this project better.

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## How to Contribute

We welcome contributions in many forms:

### Reporting Issues

Before reporting an issue, please search the [existing issues](https://github.com/programmingcorporate/PowerAppsComponents/issues) to avoid duplicates.

When reporting a bug, please include:
- Clear description of the issue
- Steps to reproduce the problem
- Expected behavior
- Actual behavior
- Your environment (PowerApps version, browser, OS)
- Screenshots or error messages (if applicable)

### Suggesting Enhancements

Enhancement suggestions are tracked as [GitHub issues](https://github.com/programmingcorporate/PowerAppsComponents/issues). When suggesting an enhancement:

1. Use a clear and descriptive title
2. Provide a detailed description of the suggested enhancement
3. Explain why this enhancement would be useful
4. List some examples of how the enhancement would be used

### Contributing Code

#### Getting Started

1. **Fork the repository** - Click the "Fork" button on GitHub
2. **Clone your fork** locally
   ```bash
   git clone https://github.com/YOUR-USERNAME/PowerAppsComponents.git
   cd PowerAppsComponents
   ```
3. **Add upstream remote**
   ```bash
   git remote add upstream https://github.com/programmingcorporate/PowerAppsComponents.git
   ```

#### Creating a Feature Branch

1. **Update your main branch**
   ```bash
   git fetch upstream
   git checkout main
   git merge upstream/main
   ```
2. **Create a feature branch**
   ```bash
   git checkout -b feature/ComponentName
   ```

#### Making Changes

1. Make your changes following the [Code Standards](#code-standards)
2. Test your changes thoroughly
3. Ensure your code follows project conventions
4. Update documentation as needed

#### Code Standards

**Component Naming:**
- Use PascalCase for component names
- Names should clearly describe the component's purpose
- Example: `HeaderComponent`, `BreadcrumbNavigation`

**Properties and Methods:**
- Use camelCase for properties and methods
- Document all properties with descriptions
- Provide clear examples of usage

**Documentation:**
- Include inline comments for complex logic
- Provide usage examples in component documentation
- Update README if adding new features

**Testing:**
- Test components on different screen sizes
- Test on different browsers (if applicable)
- Test with different data scenarios
- Ensure accessibility (keyboard navigation, screen readers)

#### Commit Messages

Follow conventional commit format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types:**
- `feat` - A new feature
- `fix` - A bug fix
- `docs` - Documentation changes
- `style` - Code style changes (formatting, missing semicolons, etc.)
- `refactor` - Code refactoring without feature changes
- `perf` - Performance improvements
- `test` - Adding or updating tests
- `chore` - Build process, dependencies, or tooling changes

**Examples:**
```
feat(header): Add logo image support to header component

fix(breadcrumb): Correct navigation on mobile screens

docs: Update component installation guide

chore: Update dependencies to latest versions
```

#### Pushing Your Changes

1. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat(ComponentName): Add new feature"
   ```

2. **Push to your fork**
   ```bash
   git push origin feature/ComponentName
   ```

#### Opening a Pull Request

1. Go to the [original repository](https://github.com/programmingcorporate/PowerAppsComponents)
2. Click "New Pull Request"
3. Select your fork and branch
4. Fill in the PR description with:
   - **What:** Brief description of changes
   - **Why:** Motivation for the changes
   - **How:** Technical approach taken
   - **Testing:** How you tested the changes
   - **Related Issues:** Links to related issues (use `Fixes #123`)

### Code Review Process

**Expectations:**
- Be open to constructive feedback
- Respond to review comments within a reasonable timeframe
- Make requested changes or discuss alternative approaches
- Tests must pass before merging
- Code must follow project standards

**Reviewers will check:**
- Code quality and style compliance
- Functionality and correctness
- Documentation completeness
- Performance implications
- Security considerations

## View-Only Policy

⚠️ **Important:** This repository is maintained by Corporate Programming and follows a **view-only** contribution policy for the main codebase.

**What this means:**
- Bug reports and feature suggestions are welcome and appreciated
- Code contributions are welcome for review and discussion
- Final decision on merging lies with the project maintainers
- Your ideas help improve the project even if not directly merged

**Your contributions matter:**
Even if your exact code isn't merged, your suggestions influence the project's direction and help us identify improvements.

## Attribution

Contributors will be recognized in:
- Pull Request discussions
- CHANGELOG.md for significant contributions
- GitHub Contributors page
- Project documentation

## Development Guidelines

### Component Development

1. **Modularity** - Create self-contained, reusable components
2. **Naming** - Use clear, descriptive names
3. **Documentation** - Every component needs usage examples
4. **Testing** - Test across different scenarios
5. **Accessibility** - Follow WCAG 2.1 standards

### Testing Your Changes

Before submitting:
1. Test on different screen sizes
2. Verify all properties work as expected
3. Check for edge cases
4. Ensure backward compatibility (when applicable)

## Questions?

- 📖 Check the [README](README.md) and [Documentation](https://github.com/programmingcorporate/PowerAppsComponents/wiki)
- 💬 Start a [Discussion](https://github.com/programmingcorporate/PowerAppsComponents/discussions)
- 📧 Contact the maintainers

## License

By contributing to PowerApps Components, you agree that your contributions will be licensed under the MIT License.

---

**Thank you for contributing to PowerApps Components!** 🎉

We appreciate your time, effort, and ideas. Together, we can build a better library for the PowerApps community.
