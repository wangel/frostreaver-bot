# Changelog

All notable changes to **Frostreaver.Bot** are documented here.

When the running bot's version changes, it posts a short note (these highlights +
a link back to this file) in each server's configured bonus channel.

## [0.4.0]

### Changed
- **`/watch <zone> <bonus>`** is now a single command — no more picking a
  `zone` / `category` subcommand first. `/unwatch <zone> <bonus>` mirrors it.
- The same flattening applies to server-wide watches: **`/guildwatch`** and
  **`/guildunwatch`** now take the zone and bonus directly.

### Added
- **`/subscribe <bonus>`** / **`/unsubscribe <bonus>`** — opt into a daily digest
  of *every* zone with a given bonus (this is what `/watch category` used to do).
  Server admins get **`/guildsubscribe`** / **`/guildunsubscribe`**.
- **`/unwatchall`** and **`/guildunwatchall`** — clear every watch and
  subscription at once (with a confirmation prompt).
- **Update announcements** — on a version bump the bot posts what's new to each
  configured channel and links here.

### Fixed
- Zone autocomplete for `/watch` no longer goes blank if the API briefly returns
  an empty zone list — the previous good cache is kept instead of being wiped.

[0.4.0]: https://github.com/wangel/frostreaver-bot/releases/tag/v0.4.0
