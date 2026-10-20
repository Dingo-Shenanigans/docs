# ReSkate docs

The documentation site for [ReSkate](https://github.com/Dingo-Shenanigans/ReSkate): getting started, and
the plugin system's guides and API. It is a [Mintlify](https://mintlify.com) site: pages are MDX files,
and `docs.json` holds the navigation, colours and links.

- `index.mdx`, `quickstart.mdx`: the home page and Getting started.
- `plugins/`: the Plugins tab. `AGENTS.md` has the rules for these pages: every function documented
  from the ReSkate source, with its exact arguments, limits and permission.

## Preview

Run this at the root, beside `docs.json`, then open `http://localhost:3000`:

```
npx mint dev
```

Before pushing, check the build and the links:

```
npx mint validate
npx mint broken-links
```

Changes are published when they reach the default branch.
