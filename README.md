# 💡 PowerApps Components Library

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)](#)
[![PowerApps](https://img.shields.io/badge/PowerApps-Enterprise-blue.svg)](#)

A professional reusable PowerApps components library featuring enterprise-grade UI controls, navigation patterns, and logic blocks. Designed for rapid development and seamless integration.

## 📋 Table of Contents

- [Overview](#overview)
- [Components](#components)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Component Documentation](#component-documentation)
- [Best Practices](#best-practices)
- [Contributing](#contributing)
- [License](#license)

## 🌟 Overview

PowerApps Components Library provides production-ready, tested components to accelerate PowerApps development. Each component follows Microsoft best practices and includes:

- **Reusable Architecture** - Use across multiple apps
- **Enterprise Features** - Responsive, accessible design
- **Well-Documented** - Clear usage instructions
- **Easy Integration** - Drag-and-drop functionality
- **Best Practices** - Following Microsoft standards

## 🚧 Components

### Available Components

| Component | Purpose | Status |
|-----------|---------|--------|
| Header Component | App header with branding | ✅ Available |
| Breadcrumb Navigation | Hierarchical navigation | ✅ Available |
| Footer Controls | App footer | 🚄 Coming Soon |
| Tabbed Navigation | Tab-based navigation | 🚄 Coming Soon |
| Custom Input Forms | Reusable form controls | 🚄 Coming Soon |
| Logic Snippets | Reusable formulas | 🚄 Coming Soon |

### Planned Components

- Enhanced data visualization components
- Advanced form validation controls
- Custom theming system
- Accessibility-first design patterns

## 📋 Prerequisites

Before using these components, ensure you have:

- PowerApps Studio installed (latest version)
- Power Platform environment access
- Microsoft 365 account or Dynamics 365 account
- Basic understanding of PowerApps and Power FX formulas

## 🔧 Installation

### Method 1: Direct Import

1. Download the `.msapp` file from the [Releases](https://github.com/programmingcorporate/PowerAppsComponents/releases) section
2. Open PowerApps Studio
3. Open the file to extract components
4. Export the components you need to your target app

### Method 2: Copy-Paste Components

1. Clone or download this repository
2. Open PowerApps Studio
3. Create a new blank app
4. Import the `.msapp` file
5. Copy components from the source app
6. Paste into your target app

### Method 3: Reference from Solution

1. Import the managed solution (when available)
2. Reference components from the solution
3. Use components across your environment

## 💡 Usage

### Basic Component Usage

```
1. Open your PowerApps app
2. Go to Components section
3. Expand the component library
4. Drag Header Component onto your screen
5. Configure properties through the Properties panel
6. Customize styling and behavior as needed
7. Test in preview mode before publishing
```

### Component Properties

Each component exposes configurable properties for customization:

- **Display Properties** - Title, icons, visibility
- **Behavior Properties** - OnSelect, OnChange events
- **Styling Properties** - Colors, fonts, sizing
- **Data Properties** - DataSource, Value bindings

### Common Patterns

**Pattern 1: Header + Content + Footer**
```
1. Add Header Component at top
2. Add content controls in middle section
3. Add Footer Component at bottom
4. Use Breadcrumb for navigation hierarchy
```

**Pattern 2: Tabbed Interface**
```
1. Use Tabbed Navigation component
2. Create screens for each tab
3. Link navigation to screen transitions
4. Maintain context across tabs
```

## 📚 Component Documentation

### Header Component

**Purpose:** Consistent application branding and primary navigation

**Properties:**
- `AppName` (Text) - Application title
- `ShowMenu` (Boolean) - Toggle menu visibility
- `BackgroundColor` (Color) - Header background
- `LogoUrl` (Text) - Logo image URL

**Events:**
- `OnMenuSelect` - Triggered when menu item selected
- `OnLogoSelect` - Triggered when logo clicked

**Example:**
```
Insert Header Component
Set AppName = "My PowerApp"
Set ShowMenu = true
Set OnMenuSelect = Navigate(Screen2)
```

### Breadcrumb Component

**Purpose:** Display hierarchical navigation path

**Properties:**
- `Items` (Table) - Array of breadcrumb items
- `Separator` (Text) - Path separator character
- `TextColor` (Color) - Breadcrumb text color

**Events:**
- `OnItemSelect` - Triggered when breadcrumb item clicked

**Example:**
```
Insert Breadcrumb Component
Set Items = Table({Label: "Home", Value: 1}, {Label: "Products", Value: 2})
Set OnItemSelect = Navigate(Screen1, ScreenTransition.Fade)
```

## 🎯 Best Practices

### Component Design

- **Keep components focused** - Single responsibility principle
- **Use clear naming** - Component names should describe purpose
- **Document properties** - Provide clear documentation for all properties
- **Test thoroughly** - Test on different screen sizes and browsers
- **Follow accessibility** - Ensure components are accessible (WCAG 2.1)

### Implementation Guidelines

1. **Naming Convention**
   - Use PascalCase for component names
   - Use camelCase for component properties
   - Use descriptive names that indicate purpose

2. **Properties Management**
   - Group related properties together
   - Provide sensible defaults
   - Document property constraints

3. **Event Handling**
   - Use consistent naming for events
   - Document expected parameters
   - Handle edge cases gracefully

4. **Documentation**
   - Include usage examples
   - Provide property descriptions
   - Document limitations and known issues

### Performance Considerations

- Minimize formula complexity in components
- Use variables instead of repeated calculations
- Test performance with large datasets
- Monitor app load times

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on:

- Reporting issues
- Suggesting enhancements
- Submitting pull requests
- Code standards and conventions

### Contribution Process

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/ComponentName`)
3. Make your changes and test thoroughly
4. Commit with clear messages (`git commit -m "feat: Add new component"`)
5. Push to the branch (`git push origin feature/ComponentName`)
6. Open a Pull Request with description of changes

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

MIT License - Free for personal, educational, and commercial use.

## 👥 Author

**Corporate Programming**

- 🌐 Website: [corporateprogramming.com](https://www.corporateprogramming.com)
- 💼 LinkedIn: [Corporate Programming](https://www.linkedin.com/company/corporateprogramming)
- 📺 YouTube: [@corporateprogramming](https://www.youtube.com/@corporateprogramming)
- 🐙 GitHub: [@programmingcorporate](https://github.com/programmingcorporate)

## 📞 Support

For issues, questions, or suggestions:

- Open an [Issue](https://github.com/programmingcorporate/PowerAppsComponents/issues)
- Check [Discussions](https://github.com/programmingcorporate/PowerAppsComponents/discussions)
- Review [Documentation](https://github.com/programmingcorporate/PowerAppsComponents/wiki)

## 🔗 Useful Resources

- [Microsoft PowerApps Documentation](https://docs.microsoft.com/en-us/powerapps/)
- [Power Platform Community](https://powerusers.microsoft.com/)
- [Canvas App Best Practices](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/performance-tips)
- [PowerApps Formula Reference](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/formula-reference)
- [Component Best Practices](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/component-best-practices)

---

**Last Updated:** February 2026
