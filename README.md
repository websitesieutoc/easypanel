# Easypanel SDK

This is an unofficial sdk for [Easypanel](https://easypanel.io) .


## Installation

```bash
pnpm install -E @sieutoc/easypanel
```

## Usage

```ts
import { easypanel } from '@sieutoc/easypanel'

const app = easypanel({
  endpoint: process.env.EASYPANEL_URL || '',
  token: process.env.EASYPANEL_TOKEN || '',
})

const project = await app.projects.create({ name: 'NewProject' })
```

## Development

Requires [pnpm](https://pnpm.js.org/) >= 8.10.0
Requires [node](https://nodejs.org/en/) >= 20.0.0

```bash
pnpm install
pnpm dev # watch mode tsup
pnpm build # build
```
