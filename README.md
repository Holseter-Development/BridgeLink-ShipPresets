# BridgeLink Ship Presets

Community-maintained ship and role presets for **BridgeLink**, a structured voice-ops app for Star Citizen fleets.

> **TL;DR**
>
> - This repo holds `shipTemplates.json` - the stock ship/role layouts BridgeLink ships with.
> - Found a wrong seat, missing ship, or bad role label? [Open an issue](../../issues).
> - Want to add or fix a ship yourself? Fork, edit the JSON, [open a PR](../../pulls).
> - Not official Star Citizen data - these are gameplay-oriented presets, not ship schematics.

## What is BridgeLink?

BridgeLink is a voice-operations app built for large, organized Star Citizen fleets. Instead of dumping everyone into one flat voice channel, it gives each crew member a role-based station: you can talk locally to your own cockpit or department, report up to your lead, command down to people under you, or broadcast fleet-wide if you have the authority. It's built around how fleets actually run operations - squads, ship departments, turret crews, boarding teams, capital ship command structures - not just "everyone in one Discord call."

This repo is the public, editable home of the ship data that powers that role structure.

## What's in this repo

`shipTemplates.json` defines, for every supported ship:

- Its manufacturer, category, and default callsign
- Tags used for matching it to operation types (combat, salvage, mining, escort, etc.)
- Its crew structure - groups of seats (Cockpit, Turrets, Engineering, Boarding Party, etc.) and the role assigned to each seat

These presets are intentionally gameplay-focused rather than 1:1 with official ship loadouts. A seat layout that makes voice communication clear and playable is preferred over strict simulation accuracy. Users can also edit and create ships from scratch inside BridgeLink itself - this file is just the stock starting set.

## Found a mistake?

Please report it. Common things worth flagging:

- Wrong or missing seats (e.g. a turret that doesn't exist, a missing co-pilot seat)
- A ship in the wrong category or with unhelpful operation tags
- Confusing or inconsistent role labels

**[Open an issue](../../issues)** with the ship name and what's wrong. Screenshots or in-game seat counts are appreciated but not required.

## Want to add a ship or fix one yourself?

Pull requests are welcome.

1. Fork this repo.
2. Add or edit an entry in `shipTemplates.json`, following the structure of existing ships (`id`, `name`, `manufacturer`, `category`, `operationTags`, `groups` → `slots`).
3. Keep `id` values lowercase, hyphenated, and unique.
4. Every ship needs at least one `pilot` role marked `isLead: true` unless it genuinely has no pilot seat.
5. Open a PR describing what changed and why.

Small, focused PRs (one ship, or a handful of related fixes) are easiest to review and merge quickly.

## Disclaimer

This is an unofficial, fan-made project. It is not affiliated with or endorsed by Cloud Imperium Games or Roberts Space Industries. Ship names and manufacturers are used for identification purposes only.

## Support

BridgeLink is a passion project - built and maintained for the Star Citizen community, with no company, ads, or paywall behind it. If it earns a place in your fleet&rsquo;s ops and you&rsquo;d like to chip in towards keeping the servers running, it genuinely helps.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/W7W6ESW2K)
