# Nuxt 3 Static Site + Wasmer

This example shows how to statically generate a **Nuxt 3** app and host it on **Wasmer Edge**.

> Nuxt’s full server-side rendering story for Wasmer (via WinterJS) is in progress. For now, this template targets **`npm run generate`** so you can deploy a pre-rendered site.

## Demo

https://nuxt-starter-wasmer-examples.wasmer.app/

## How it Works

Key pieces of the starter:

* `app.vue` and components under `components/` render the UI.
* `nuxt.config.ts` uses the default static target; when you run `npm run generate` the site is output to `.output/public`.
* The static folder is served directly by Wasmer Edge, so no serverless functions are required.

Add pages under `pages/` or use content modules as usual—just make sure everything can be generated ahead of time.

## Running Locally

```bash
npm install
npm run dev
```

Visit `http://127.0.0.1:3000/` for the dev server. To preview the generated output Wasmer will get:

```bash
npm run generate
npm run preview
```

## Deploying to Wasmer (Overview)

1. Run `npm run generate` to emit the static site into `.output/public`.
2. Configure Wasmer Edge to publish `.output/public` (or copy it to a `dist/` directory).
3. Deploy and browse `https://<your-subdomain>.wasmer.app/`.
