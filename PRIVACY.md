# Frostreaver.Bot — Privacy Policy

_Last updated: 2026-05-27_

This policy describes what data Frostreaver.Bot ("the bot") collects, why, and how long it's kept. The bot is operated by **wangel** (the "operator") and is a free, non-commercial project.

## What the bot collects

The bot only stores the **minimum** data it needs to deliver notifications you explicitly opt into.

When you run a `/watch` or `/guildwatch` command, the bot stores:

- Your **Discord user ID** (if a personal watch) or the **Discord server ID** (if a guild watch).
- The **bonus type** and/or **zone name** you asked to be notified about.

When a server admin runs `/setchannel`, the bot stores:

- The **Discord server ID** and the **channel ID** where notifications should be posted.

The bot also keeps short-lived deduplication records (subject, bonus, zone, date) so it doesn't ping you twice for the same event in the same day. These are pruned automatically once the day passes.

## What the bot does NOT collect

- **No message content.** The bot does not read messages.
- **No member lists.** The bot does not enumerate or store the members of any server.
- **No usernames, avatars, emails, or other profile data.**
- **No analytics, tracking pixels, or third-party telemetry.**

## Logs

The bot writes operational logs (errors, slash-command invocations, joined/left guild events) for debugging and abuse monitoring. These logs may include your Discord user ID and the command you ran. Logs are stored on the operator's server, rotate automatically, and are retained for at most a few days before being overwritten.

## Where data is stored

All persistent data is stored in a local SQLite database on a server the operator controls. The bot does not transmit data to any third party other than:

- **Discord** — to deliver messages and respond to interactions, as required for the bot to function.
- **frostreaver.zone** — the bot fetches public bonus-zone data from this site. No user data is sent in those requests.

## Deleting your data

- **Per-watch:** `/unwatch zone`, `/unwatch category`
- **Everything personal:** `/unwatch all`
- **Server data:** an admin can run `/guildunwatch all` and remove the bot from the server.
- **Need a manual wipe?** Contact wangel on Discord.

Removing the bot from a server, or uninstalling the user-app, does not automatically purge prior watches — run the unwatch commands above, or contact the operator.

## Children

The bot is not directed at children under 13. The bot collects no information that could identify a child.

## Changes

This policy may be updated. The "Last updated" date above will reflect the most recent change.

## Contact

Questions or data-deletion requests? Reach out to **wangel** on Discord.
