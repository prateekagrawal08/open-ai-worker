# open-ai-worker

## Create a Worker

```sh
npm create cloudflare@latest
```

This scaffolds a new Worker project.

## Prepare for Deployment

Before deploying, ensure your project includes:

- **Worker script**: e.g., `src/index.js` with your worker logic. Learn how to write a Worker at the [Workers Getting Started guide](https://developers.cloudflare.com/workers/get-started/guide/).
- **wrangler.toml configuration**: defines deployment settings. Create a `wrangler.toml` at your project root:

```toml
name = "my-worker"
main = "src/index.js"
compatibility_date = "2024-01-01"
```

See [Wrangler configuration documentation](https://developers.cloudflare.com/workers/wrangler/configuration/) for details.

## Deploy a Worker

```sh
npx wrangler deploy
```
