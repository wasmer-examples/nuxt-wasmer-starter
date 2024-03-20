
This is a [Nuxt 3](https://nuxt.com) starter project.

> Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

> [!IMPORTANT]
> Support for running Nuxt fully server-side with Wasmer using [WinterJS](https://github.com/wasmerio/winterjs) is on the works. Meanwhile you can serve the static website via `npm run build`.

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
wasmer run wasmer-examples/nuxt-wasmer-starter --net -- --port 3000
```

> [!TIP]
> You can also run `wasmer run . --net -- --port 3000` in the root of this repo, after running `npm run build`


Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.


## Deploy on Wasmer Edge

The easiest way to deploy your Nuxt app is to use the [Wasmer Edge](https://wasmer.io/products/edge).

Live example: https://wasmer-edge-nuxt-ssg-sample.wasmer.app/

First, you'll need to run `npm run build`, and then, to deploy to Wasmer Edge:

```bash
wasmer deploy
```

> [!NOTE]
> You will need to have Wasmer installed (check out [the docs to install the Wasmer CLI](https://docs.wasmer.io/install)!). 
> You will also need to change the namespace in `wasmer.toml` to your own namespace and app name in `app.yaml` to your own app name.
