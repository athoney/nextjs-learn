## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.


## Folder structure info
- `/app` contains routes, components, and logic for app (most work is done here)
- `/app/lib` contains utility functions and data fetching functions
- `/app/ui` contains ui components such as cards, tables, and forms
- `public` contains static assets such as images
- `/scripts` contains a seeding script that can be used to populate the database
- config files are created with the create-next-app command and do not to be modified for this project

## Routes info
- `/app/page.tsx` is the main page for the app
- you can create seperate UIs for each route using layout.tsx and page.tsx files
   - `page.tsx` is a special Next.js file that export a React component, and it is required for the route to be accessible. 
   - `layout.tsx` is a special file to create a UI that is shared between multiple pages. (Good for a navbar or sidebar)
    - one benefit of using layouts in Next.js is that on navigation, only the page components update while the layout won't re-render. This is called partial rendering and it's good for performance.
    - `/app/layout.tsx` is the main layout for the app. This is called a root layout and is required. Any UI you add to the root layout will be shared across all pages in your application. You can use the root layout to modify your <html> and <body> tags, and add metadata (you'll learn more about metadata in a later chapter).