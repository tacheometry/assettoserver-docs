---
title: Changelog
---
## Patreon Plugins

### v0.0.36

#### PatreonDynamicSkinsPlugin (new!)

#### PatreonChatRolesPlugin (new!)

#### PatreonRaceChallengePlugin

* Fix chat commands not working

#### PatreonSafetyRatingPlugin

* Fix chat name colors on CSP <0.1.79

#### PatreonSpeedTrapPlugin

* Fix speed trap flash not showing for other players

### v0.0.35

#### PatreonSafetyRatingPlugin (new!)

This plugin calculates a safety rating based on number of collisions and driven distance. Clean drivers will get a higher rating than people crashing every corner.  
You can also set a color for each safety rating rank that will be shown in chat and name tags.

#### PatreonTimingPlugin

* Disable timing for cars marked as `AI=fixed` (admins taking these cars were able to set times on the leaderboard)

#### PatreonSpeedTrapPlugin

* Ability to customize image overlays with Lua
* Fix wrong calculation of forward vector for custom speed traps
* add new variables `Guid` and `Car` for Discord webhooks

### v0.0.34

#### PatreonTwitchChatPlugin (new!)

If you're a streamer and running your own servers, this plugin might be helpful for you. It will forward all messages from your Twitch chat to the AC ingame chat and (optionally) vice versa.

Thanks to **AEGIS | VISUALS** for commissioning this plugin!

#### PatreonSpeedTrapPlugin

* Now works with maps other than SRP, custom speed traps can be defined in the [configuration](./plugins/PatreonSpeedTrapPlugin.md#custom-speed-traps)
* Overlay and grayscale can be disabled
* Allow players to disable picture upload, can help with slow internet connections

#### PatreonReservedSlotsPlugin

* Configuration has been updated to allow reserving specific entry list slots
* Using the new AssettoServer Hub user groups, it is possible to sync reserved slots across all your game servers

:::caution Breaking Changes!

Please review the [documentation](./plugins/PatreonReservedSlotsPlugin.md).

:::

## AssettoServer Hub

### v0.0.6

#### Timing Leaderboard
* Add filter for current month
* Add API
* Do not show tracks with no lap times set

#### Discord
* Add Discord Bot
* Add ability to link Steam account to Discord account
* Add Discord role mappings
* Add server status embeds

### v0.0.5

* Add race challenge leaderboard
* Improvements to timing leaderboards
* Add support for safety ratings
* Updated to .NET 7
* Fix menu not working on mobile

### v0.0.4

* Added a web interface for timing leaderboards ([demo](https://demo.assettoserver.org/timing))
* Introduced a new concept called user groups, making it possible to have multiple whitelists/blacklists and sync all lists to your game servers

:::caution Breaking changes!

Synchronizinig blacklist/whitelist to your game servers requires new configuration, please check the [documentation](./assettoserver-hub/index.md#how-to-sync-user-groups-from-the-hub-to-your-game-servers).

:::