## TUTORIAL

`https://youtu.be/NgayZAuTgwM?si=XZzIQU03YBj-fnV8`

- LOOK ALSO: `D:\APPLICATIONS\max\_coding\NEXT.JS\nextjs-nestjs-prisma-docker`

## INSTALLATION

- NEXT.JS
  `npx create-next-app@latest my-app-name`
  Would you like to use TypeScript? ... Yes
  Would you like to use ESLint? ... Yes
  Would you like to use Tailwind CSS? ... Yes
  Would you like to use `src/` directory? ... Yes
  Would you like to use App Router? (recommended) » Yes
  Would you like to customize the default import alias (@)? » No

- PRISMA
  `npm i prisma --save-dev`
  `npx prisma init --datasource-provider sqlite`
  `npx prisma migrate dev --name init` - after completing `schema.prisma`
  ADD `"postinstall": "prisma generate"` to package.json scripts to avoid Vercel caching making Prisma Client becoming out of sync with your database schema.
  CHANGE the build script to `"build": "prisma generate && <actual-build-command>"`

### COMMANDS

RUN: `npm run dev`

### TO DO

Add to .gitignore: `.env` and `dev.db*`
