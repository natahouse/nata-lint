<h1 align="center">
  <img alt="natahouse" title="natahouse" src="https://github.com/natahouse/nata-lint/assets/44790240/3e406b45-0fe0-43d2-9204-5b22b6faac8b" />
</h1>

<p align="center">
  <a href="#-overview">Overview</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-features">Features</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-getting-started">Getting started</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-style-rules">Style rules</a>&nbsp;&nbsp;&nbsp;
</p>

## 💻 Overview

This project provides a centralized ESLint configuration for projects utilizing Next.js, React, and Node.js. 
This configuration aims to enhance code quality, enforce best practices, and streamline the development process, by maintaining a consistent set of linting rules.
<br />
<br />

## 🌟 Features
```diff
@@ Next.js Ready: @@ 
Tailored rules for projects built with Next.js,
ensuring optimal linting for Next.js applications.

@@ React Guidelines: @@ 
Comprehensive linting rules specific to React, 
promoting clean and maintainable React code.

@@ Node.js Support: @@
Inclusive rules for Node.js applications, addressing common issues 
and ensuring code consistency across the full stack.

@@ Easy Integration: @@
Straightforward integration into your project, saving
development time and reducing configuration overhead.
```
<br />

## 🚀 Getting Started

To integrate this ESLint configuration into your project, follow these steps:

```bash
## Use your preferred package manager to install
$ yarn add -D @natahouse/lint-config
## OR
$ npm install --save-dev @natahouse/lint-config
```
---
#### Using in ReactJS (without NextJS)
inside the `.eslintrc.json` file
```json
{
  "extends": "@natahouse/lint-config/react"
}
```
---
#### Using in NextJS
inside the `.eslintrc.json` file
```json
{
  "extends": [
    "@natahouse/lint-config/next",
    "next/core-web-vitals",
  ]
}
```
---
#### Using in NodeJS
inside the `.eslintrc.json` file
```json
{
  "extends": "@natahouse/lint-config/node"
}
```
---
<br />

## 🎨 Style rules


#### Prettier Configuration
The following table outlines the configuration rules for [Prettier](https://prettier.io/), a code formatter.

| Rule                       | Value        | Description                                           |
| -------------------------- | ------------ | ----------------------------------------------------- |
| `printWidth`               | 80           | Specifies the maximum line length for your code.      |
| `tabWidth`                 | 2            | Sets the number of spaces per indentation level.      |
| `singleQuote`              | false        | Controls the usage of single or double quotes.        |
| `trailingComma`            | "all"        | Adds a trailing comma wherever possible (ES5+).       |
| `arrowParens`              | "always"     | Enforces parentheses around a sole arrow function     |
| `semi`                     | true         | Adds semicolons at the end of statements.             |
| `endOfLine`                | "auto"       | Defines the line ending style for your files.         |

---

#### ESLint Configuration for ReactJS
This ESLint configuration is tailored for projects using React.js, providing a set of rules to enhance code quality, enforce best practices, and improve maintainability. It extends popular configurations such as `plugin:react/recommended`, `plugin:react-hooks/recommended`, `standard`, `plugin:@typescript-eslint/recommended`, and `plugin:prettier/recommended`.

| Rule                                     | Value   | Description                                                                                       |
| ---------------------------------------- | ------- | ------------------------------------------------------------------------------------------------- |
| `react/self-closing-comp`                | "error" | Enforces self-closing components in React to improve consistency.                                 |
| `react/react-in-jsx-scope`               | "off"   | Allows JSX to be used without importing React explicitly (not necessary in newer React versions). |
| `react/prop-types`                       | "off"   | Disables the requirement for prop types in React components, suitable for TypeScript projects.    |
| `jsx-a11y/alt-text`                      | "warn"  | Warns about missing `alt` text in `img` elements with optional elements customization.            |
| `jsx-a11y/aria-props`                    | "warn"  | Warns about problematic usage of ARIA props.                                                      |
| `jsx-a11y/aria-proptypes`                | "warn"  | Warns about missing ARIA propTypes.                                                               |
| `jsx-a11y/aria-unsupported-elements`     | "warn"  | Warns about unsupported ARIA elements.                                                            |
| `jsx-a11y/role-has-required-aria-props`  | "warn"  | Warns about missing required ARIA props for certain roles.                                        |
| `jsx-a11y/role-supports-aria-props`      | "warn"  | Warns about unsupported ARIA props for certain roles.                                             |
| `react/no-unknown-property`              | "error" | Flags the usage of unknown DOM properties in React components.                                    |

---

#### ESLint Configuration for NextJS

This ESLint configuration is tailored for projects using Next.js, providing a set of rules to enhance code quality, enforce best practices, and improve maintainability. It extends popular configurations such as `standard`, `plugin:@typescript-eslint/recommended`, and `plugin:prettier/recommended`.

| Rule                                     | Value   | Description                                                                                   |
| ---------------------------------------- | ------- | --------------------------------------------------------------------------------------------- |
| `prettier/prettier`                      | "error" | Prettier configuration for consistent code formatting.                                        |
| `jsx-a11y/alt-text`                      | "warn"  | Warns about missing `alt` text in `img` elements with optional elements customization.        |
| `jsx-a11y/aria-props`                    | "warn"  | Warns about problematic usage of ARIA props.                                                  |
| `jsx-a11y/aria-proptypes`                | "warn"  | Warns about missing ARIA propTypes.                                                           |
| `jsx-a11y/aria-unsupported-elements`     | "warn"  | Warns about unsupported ARIA elements.                                                        |
| `jsx-a11y/role-has-required-aria-props`  | "warn"  | Warns about missing required ARIA props for certain roles.                                    |
| `jsx-a11y/role-supports-aria-props`      | "warn"  | Warns about unsupported ARIA props for certain roles.                                         |

---

Made with ♥ by <a href="https://natahouse.com" target="_blank">nata.house</a> 👋🏻
