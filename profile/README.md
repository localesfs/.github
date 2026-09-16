<p align="center">
  <img src="logo.png" width="120" height="120" alt="LocalesFS" />
</p>

<h1 align="center">LocalesFS</h1>

<p align="center">
  <strong>Translations that ship with the product.</strong><br />
  Import locale files, draft with AI, review with your team, and export when the copy is ready.
</p>

<p align="center">
  <a href="https://localesfs.com">localesfs.com</a> ·
  <a href="https://localesfs.com/docs">Docs, guides &amp; API</a> ·
  <a href="mailto:alex@bitscorp.co">Contact</a>
</p>

---

LocalesFS lives at [localesfs.com](https://localesfs.com). Documentation, plugin guides, and the REST API are at [localesfs.com/docs](https://localesfs.com/docs). This GitHub org holds the platform, plugins, and client SDKs.

### Platform

| Repository | What it is |
|---|---|
| [`locales`](https://github.com/locales-app/locales) | Core product — API, dashboard, billing, AI translation |
| [`localesfs-github`](https://github.com/locales-app/localesfs-github) | GitHub App for repo import / sync |
| [`localesfs-sdk`](https://github.com/locales-app/localesfs-sdk) | TypeScript SDK + CLI (`npx @localesfs/sdk`) |

### CMS plugins

Install, push source strings, translate in LocalesFS, pull them back.

| Repository | Install |
|---|---|
| [`localesfs-wordpress`](https://github.com/locales-app/localesfs-wordpress) | WordPress plugin — Settings → LocalesFS |
| [`localesfs-contentful`](https://github.com/locales-app/localesfs-contentful) | `npx @localesfs/contentful push` / `pull` |
| [`localesfs-shopify`](https://github.com/locales-app/localesfs-shopify) | `npx @localesfs/shopify push` / `pull` |
| [`localesfs-strapi`](https://github.com/locales-app/localesfs-strapi) | `npm install @localesfs/strapi` |

### Mobile

Bundle locales at build time, then `t("key")` in the app.

| Repository | Client |
|---|---|
| [`localesfs-react-native`](https://github.com/locales-app/localesfs-react-native) | React Native / Expo |
| [`localesfs-flutter`](https://github.com/locales-app/localesfs-flutter) | Flutter |
| [`localesfs-ios`](https://github.com/locales-app/localesfs-ios) | Swift package |
| [`localesfs-android`](https://github.com/locales-app/localesfs-android) | Kotlin |

### Design

| Repository | What it is |
|---|---|
| [`localesfs-figma`](https://github.com/locales-app/localesfs-figma) | Figma plugin for localized frames |

---

```bash
npx @localesfs/sdk bundle --out ./locales
```

Shared API for every plugin and SDK:

```
POST /api/projects/:id/import
GET  /api/projects/:id/bundle
```

Docs: [localesfs.com/docs](https://localesfs.com/docs) · Product: [localesfs.com](https://localesfs.com)
