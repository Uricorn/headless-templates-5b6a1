# Mondial Losers of 2026

A satirical scoreboard tracking every team eliminated from the 2026 FIFA World Cup, with a roast for the road. Built on [Wix Headless](https://dev.wix.com/docs/go-headless) (Astro + Wix CMS).

**Live site:** https://mondial-lo-31f7cd21-clanroc.wix-site-host.com

## Content

Eliminated teams are stored in a Wix CMS (Wix Data) collection called `losers`, with fields for the team, flag, opponent, round, score, elimination date, and a short roast. The homepage lists every team (most recently eliminated first); each team links to its own detail page at `/losers/<slug>`.

To add or edit teams as the tournament progresses, edit the `losers` collection in the [Wix dashboard](https://manage.wix.com) (Content Manager) — the site reads it live, so changes show up with no redeploy.

## Local development

```sh
yarn install
yarn dev
```

Requires a logged-in Wix CLI session (`npx @wix/cli login`) with access to this project's site (see `wix.config.json`).

## Build & release

```sh
yarn build
yarn release
```

## Need help?

- [Wix Headless Documentation](https://dev.wix.com/docs/go-headless)
- [Wix SDK Documentation](https://dev.wix.com/docs/sdk)
- [Community on Discord](https://discord.gg/n6TBrSnYTp)
