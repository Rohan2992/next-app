This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## Why Next.js is better

### Problems In React:

- Waterfalling

  - Sending multiple backend requests to servers and getting the data and rendering it onto the browser.
  - First Time gets an empty index.html file.
  - Fetches all the .js files.
  - send the backend requests to get the user details.
  - Not a good approach.

- Not SEO Optimized

  - Search engine gets the information about the website using the HTML of the website and are not able to read the .js file.
  - Search engine are not able to know what the website is doing and how .js files are working.

- JS don't run on Emails
  - Emails can't run JS they only shows the HTML files.

### Solution:

- **Server Side Rendering**

  - First render is done on the server side and then the HTML and all the Js files along with the React code is send to the client for handling the other requests.
  - In React, SSR is done using [renderToStaticMarkup from ReactDOM/server] method.

### NEXT Features & Facts:

- Import only useful libraries on servers to keep the bundle size small.
- Needs a running server has access to the backend.
- No access to the browser constructs.
- Can't run Hooks Does not understand states.
- Let's us to write http backends no need to make express routes.
- we can write both the frontend and backend in NEXT.js
