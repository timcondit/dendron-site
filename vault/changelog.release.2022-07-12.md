---
id: 2aeg4dbvo7h9dicskivpa2x
title: 0.103
desc: ''
updated: 1658226843082
created: 1657620741057
---

Dendron 0.103 has sprouted  🌱
July 12, 2022

**Smart Note References:** Check your references! With smart note refs, a reference to a header will now include everything between the header and the next header of equal or lesser depth.
- More Information: [[enableSmartRefs|dendron://dendron.dendron-site/dendron.topic.note-reference.config.enable-smart-refs]]

### Deprecated
- `Open Link` command is deprecated as it is now merged with the [[Go to|dendron://dendron.dendron-site/dendron.ref.commands.goto]] command
- `Delete Node` command is deprecated and will be renamed to [[Delete|dendron://dendron.dendron-site/dendron.ref.commands#delete]] command

## Highlights
- feat(workspace): smart note refs

## Everything Else
- enhance(workspace): Show notice for manual migration if upgrading from from legacy versions
- enhance(navigate): `Go To` command also open external links
- enhance(workspace): remove getting started from initial tutorial
- enhance(edit): delete command also closes current window
- fix(retrieve): bad parsing of xvault wikilink with space

## Community

### Dendron Reading Series

This week's entry in the [[Dendron Reading Series|dendron://dendron.dendron-site/community.events.reading-series]].

[[How to know everything |dendron://dendron.dendron-site/community.events.reading-series.2022.07.12]]

### Event Reminders

- **Greenhouse Talks:** Visit the [[Greenhouse Talks|dendron://dendron.dendron-site/community.events.greenhouse]] for notes from previous sessions.
    - Next: [Fri, Jul 29, 04:00 PM PST / 00:00 UTC](https://link.dendron.so/luma)
    - [Greenhouse Talk Recordings - YouTube Playlist](https://link.dendron.so/greenhouse)
- **Office Hours:** Visit the [[Office Hours page|dendron://dendron.dendron-site/community.events.office-hours]] for notes from previous sessions.
    - Next: [Wed, Aug 03, 09:00 AM PST / 17:00 UTC](https://link.dendron.so/luma)
    - [Office Hour Recordings - YouTube Playlist](https://link.dendron.so/6yPa)
- **Community Teatime:** Drink tea, eat food, and hangout with the Dendron crew!
    - Next: [Thu, Jul 21, 11:00 AM PST / 19:00 UTC](https://link.dendron.so/luma)

### Thank You's

A big **thanks** to the following gardeners that brought up issues, contributions, and fixes to this release :man_farmer: :woman_farmer: 
Visit [[Discord Roles|dendron://dendron.dendron-site/community.discord.roles]] for more information.

- [Ryan Hill](https://github.com/rlh1994) `@rlh1994#9754`
    - issue with missing dependency in dendron-cli

- [Derek Ardolf](https://github.com/ScriptAutomate) `@icanteven#0264`
    - [Fix broken links; upgrade Dendron to fix Firefox experience](https://github.com/dendronhq/dendron-site/pull/587)
    - [Update referenced to deprecated dendron markdown preview enhanced extension](https://github.com/dendronhq/dendron-site/pull/588)

- [Robert van Kints](https://github.com/Sjiep)
    - #role.bugcatcher
    - [YAML validator not working on Dendron Configure (yaml)](https://github.com/dendronhq/dendron/issues/3187)

- [Patrik Grip-Jansson](https://github.com/kap42)
    - #role.bugcatcher
    - [getDayOfWeek fails](https://github.com/dendronhq/dendron/issues/3204)
    - [Minor grammar edit: "2" -> "two"](https://github.com/dendronhq/dendron-site/pull/580)

- [Jeff Hopper](https://github.com/HopperTech)
    - [Receiving "disconnect" message](https://github.com/dendronhq/dendron/issues/3212)

## Changelog
![[changelog#01030,1:#01020]]
