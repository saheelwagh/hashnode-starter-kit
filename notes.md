# Notes from github

Blog Starter Kit lets you instantly deploy a Next.js and Tailwind powered frontend for your Hashnode blog. It consumes Hashnode's Public APIs,

https://apidocs.hashnode.com/

deploy to vercel as nextjs

use personal as the root dir

set these envs 
NEXT_PUBLIC_HASHNODE_GQL_ENDPOINT=https://gql.hashnode.com
NEXT_PUBLIC_HASHNODE_PUBLICATION_HOST=engineering.hashnode.com -> Change this to your Hashnode blog URL i.e. handle.hashnode.dev
NEXT_PUBLIC_BASE_URL=/blog -> This could be /blog if you are installing on subpath; otherwise remove this var
NEXT_PUBLIC_MODE=production

for ruunug locally  
cd packages/blog-starter-kit/themes/enterprise or packages/blog-starter-kit/themes/personal
Copy .env.example to .env.local
pnpm install
pnpm dev

In the .env.local file, to display a specific blog on your website, edit the value of NEXT_PUBLIC_HASHNODE_PUBLICATION_HOST to match the URL of the Hashnode blog you want to display.
