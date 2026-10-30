---
title: Install
description: Run OxyBook locally with Docker Compose.
---

# Install

Clone the repository and start the stack:

```sh
cp .env.example .env
docker compose up -d --build
```

![The stack after start-up](images/stack.svg)

| Service  | Port | Role                  |
| -------- | ---- | --------------------- |
| app      | 3000 | API and editor        |
| worker   | 3001 | sync, builds          |
| caddy    | 8080 | serves built sites    |

:::warning Keep the secret key
Changing `OXYBOOK_SECRET_KEY` after the GitHub App is stored makes the server refuse to start.
:::

Next: [Configure](configure.mdx).
