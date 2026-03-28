# ezyExpress-CLI🚀

[![npm version](https://img.shields.io/npm/v/celexpress)](https://www.npmjs.com/package/celexpress)
[![Node.js version](https://img.shields.io/node/v/celexpress)](https://nodejs.org/)
[![License](https://img.shields.io/github/license/<USERNAME>/celexpress)](LICENSE)

**exyExpres** — *Fast & Simple Express.js Project Generator CLI*

---

## Table of Contents

1. [Overview](#overview)
2. [Installation](#installation)
3. [Usage](#usage)
4. [CLI Commands](#cli-commands)
5. [Project Folder Structure](#project-folder-structure)
6. [Templates](#templates)
7. [Configuration](#configuration)
8. [Contribution](#contribution)
9. [License](#license)
10. [Roadmap](#roadmap)

---

## Overview

Celexpress is a CLI tool for quickly scaffolding **Express.js projects**. It provides **Artisan-style commands** to generate controllers, models, routes, and middlewares with ease.

* Fast project setup
* Interactive prompts
* JS & TypeScript support
* Modular and extendable CLI

---

## Installation

**Run via npx (no install required):**

```bash
npx ezyexpres
```

**Global installation (optional):**

```bash
npm install -g ezyexpres
cex
```

> `cex` is the CLI shortcut for Celexpress commands.

---

## Usage

### Create a new project

```bash
ezyexpres create my-app
```

Interactive prompts:

```text
📂 Project name? my-app
📝 Use TypeScript? (y/N) n
📁 Select folders: routes, controllers, models, middlewares, services
```

### Generate files

```bash
# Generate a controller
ezyexpres make:controller UserController

# Generate a model
ezyexpres make:model User

# Generate a route
ezyexpres make:route user

# Generate middleware
ezyexpres make:middleware auth

# Generate service
ezyexpres make:service UserService
```

---

## CLI Commands

| Command                      | Description                    |
| ---------------------------- | ------------------------------ |
| `ezyexpres create <project-name>`  | Scaffold a new Express project |
| `ezyexpres make:controller <name>` | Generate a controller file     |
| `ezyexpres make:model <name>`      | Generate a model file          |
| `ezyexpres make:route <name>`      | Generate a route file          |
| `ezyexpres make:middleware <name>` | Generate middleware file       |
| `ezyexpres make:service <name>`    | Generate service file          |
| `ezyexpres --help`                 | List all commands              |

---

## Project Folder Structure

```text
celexpress/
├── bin/
│   └── celexpress.js
├── commands/
│   ├── create.js
│   ├── makeController.js
│   ├── makeModel.js
│   ├── makeRoute.js
│   └── makeMiddleware.js
├── templates/
│   ├── js/
│   │   ├── server.js
│   │   ├── controller.js
│   │   └── route.js
│   └── ts/
│       ├── server.ts
│       ├── controller.ts
│       └── route.ts
├── utils/
│   └── fileHelpers.js
├── config/
│   └── defaultConfig.json
├── package.json
├── README.md
├── .gitignore
└── LICENSE
```

---

## Templates

**JS Templates (`templates/js/`)**

* `server.js` → basic Express server
* `controller.js` → sample controller
* `route.js` → basic route

**TS Templates (`templates/ts/`)**

* `server.ts` → TypeScript server
* `controller.ts` → TypeScript controller
* `route.ts` → TypeScript route

---

## Configuration

Default configuration file: `config/defaultConfig.json`

```json
{
  "useTypeScript": false,
  "defaultFolders": ["routes","controllers","models","middlewares","services","config","utils"]
}
```

---

## Contribution

1. Fork the repository
2. Clone locally: `git clone https://github.com/<USERNAME>/celexpress.git`
3. Install dependencies: `npm install`
4. Create a new branch for your feature: `git checkout -b feature/<name>`
5. Commit your changes and submit a pull request

---

## License

MIT License © 2026 <San Tola>

---

## Roadmap

* **v1.0**: JS scaffolding, basic make commands
* **v1.1**: TypeScript support, auto `.env` creation, middleware templates
* **v1.2**: Database scaffolding, logging setup
* **v2.0**: Plugin system, multi-framework support

---

**ezyExpres-cli** — *Fast & Simple Express.js Project Generator CLI*
