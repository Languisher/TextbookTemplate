# Textbook

Markdown files should be placed inside of the `src/` folder.

## Running locally

> [!NOTE]  
> Running this project locally requires **node v20** or greater. [See here](https://nodejs.org/en/download/package-manager) for installation instructions.

Install and run:

```bash
npm install
npm run dev
```

and then open [http://localhost:3000](http://localhost:3000) with your browser.

## Configurations

In `app/book.tsx`, find:

```tsx
  const meta: NodeMetadata = {
    ...result.data,
    nodePath,
    contentPath,
    path: browserPath,
    nav_title: result.data.nav_title ?? result.data.title,
    hidden: result.data.hidden ?? false,
    github: `https://github.com/Languisher/TextbookTemplate/blob/main/${contentPath}`, // Change here !!
  };
```

## Change Placeholders

Change the `TITLEPLACEHOLDER`. Use search to locate its place and replace with your actual title name.