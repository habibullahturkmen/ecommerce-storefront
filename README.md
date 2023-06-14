# Next.js 13 ECommerce Storefront

- Performant by default
- SEO Ready
- Internationalization
- Responsive
- UI Components
- Theming
- Standardized Data Hooks
- Integrations - Integrate seamlessly with the most common ecommerce platforms.
- Dark Mode Support
- TailwindCSS, Next.js Page Router

## Integrations

Vendure 2.0 integrated

## Considerations

- `packages/commerce` contains all types, helpers and functions to be used as a base to build a new **provider**.
- The **Vendure Provider** live under `packages`'s root folder and it will extend Next.js Commerce types and functionality (`packages/commerce`).
- We have a **Features API** to ensure feature parity between the UI and the Provider. The UI should update accordingly and no extra code should be bundled. All extra configuration for features will live under `features` in `commerce.config.json` and if needed it can also be accessed programmatically.

## Configuration

Open `site/.env.local` and set the below values.
```
COMMERCE_PROVIDER=@vercel/commerce-vendure
NEXT_PUBLIC_VENDURE_SHOP_API_URL=http://localhost:3000/shop-api
NEXT_PUBLIC_VENDURE_LOCAL_URL=/vendure-shop-api
```


## How to run the ecommerce locally

1. Start the Vendure server first: [here](https://github.com/habibullahturkmen/ecommerce-core)
2. After that configure the env as mentioned above, go to the root of this repo, and type `pnpm i`, and `pnpm dev`
3. Vendure api in `localhost:3000`, Vendure admin in `localhost:3000/admin`, storefront in `localhost:3001`


## Demo

<img src="demo.gif" alt="demo">
<br>
<br>
<br>
