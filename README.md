# Blogger site + User Authentication & Session Management(Backend)
## Here's [Frontend repo](https://github.com/zkindest/fs-gql-rq-frontend)

## Recomended

1. [mysql vscode extension](https://marketplace.visualstudio.com/items?itemName=cweijan.vscode-mysql-client2&ssr=false#review-details)

## Available Scripts

```sh
# Generate artifacts (Prisma Client & Nexus Types)
yarn server run generate

# Generate env types(src/types/env.d.ts) from .env file
yarn server gen:env-types

yarn server dev
yarn server test
yarn server start

# Publish schema to Apollo schema registry (Needs Development server running)
# change `starter-fullstack@current` with your `graph-id@variant` in `package.json`
# more info: https://studio.apollographql.com/sandbox/explorer
yarn server run publish:schema
```

> Check [Server](./packages/server) for more info.

## Future

1. Add e2e tests
2. ~~improve token synchronization between tabs~~ ✅️

## Troubleshoot

<details>
<summary>
Cannot find module '/[redacted]/starter/.yarn/releases/yarn-berry.cjs
</summary>

```sh
rm .yarnrc.yml
yarn set version berry

# and add below line to `.yarnrc.yml`
nodeLinker: node-modules

```

</details>
