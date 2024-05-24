
This is a [Nuxt 3](https://nuxt.com) starter project.

> Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

> [!IMPORTANT]
> Support for running Nuxt fully server-side with Wasmer using [WinterJS](https://github.com/wasmerio/winterjs) is on the works. Meanwhile you can serve the static website via `npm run generate`.

## Usage

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm run dev

# yarn
yarn dev

# bun
bun run dev
```


You can also run the Nuxt template easily using Wasmer (check out the [install guide](https://docs.wasmer.io/install)):


```bash
npm run generate
wasmer run . --net -- --port 3000
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.


## Deploy on Wasmer Edge

The easiest way to deploy your Nuxt app is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: https://nuxt-starter-wasmer-examples.wasmer.app/

First, you'll need to run `npm run generate`, and then, to deploy to Wasmer Edge:

```bash
wasmer deploy
```
