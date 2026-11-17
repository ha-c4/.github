# Home Assistant + Control4 (ha-c4)

A community effort to gather the improvements to Home Assistant's Control4 support, now spread across many forks, into one shared, maintained place.

> [!IMPORTANT]
> **ha-c4 is an independent community project.** It is not affiliated with, endorsed by, or supported by the Home Assistant project, Nabu Casa, Control4, or Snap One. See the [disclaimer](#disclaimer) below.

## Why this exists

Home Assistant talks to Control4 systems through [pyControl4](https://github.com/lawtancool/pyControl4), a Python library created by [lawtancool](https://github.com/lawtancool). Over the years, many people have forked that library and the integrations built on it to add device support, fix bugs, or keep up with Control4 OS changes.

Those improvements are useful, but they are scattered:

- Fixes and features live in separate forks and often never make it upstream.
- Users have to choose one fork and give up what the others offer.
- The same problems get solved more than once, in incompatible ways.

ha-c4 hopes to bring that work back together.

## Goals

- **Collect**: find and review worthwhile changes across community forks.
- **Combine**: merge them into one tested codebase, with credit to the original authors.
- **Contribute back**: send changes upstream to pyControl4 and Home Assistant where we can, instead of drifting into yet another permanent fork.

This is an early-stage project. Expect things to change as we learn which forks and features matter most.

## Projects

| Repository | Description |
| --- | --- |
| [pyControl4](https://github.com/ha-c4/pyControl4) | Fork of [lawtancool/pyControl4](https://github.com/lawtancool/pyControl4), the Python asyncio library for Control4 systems. Combined fork changes land here. |

## Related upstream projects

- [lawtancool/pyControl4](https://github.com/lawtancool/pyControl4): the original library this work builds on.
- [Home Assistant Control4 integration](https://www.home-assistant.io/integrations/control4/): the official integration in Home Assistant core. ha-c4 does not replace it. Where possible, improvements should end up there.

## Contributing

Contributions are welcome, especially pointers to forks that already solve real problems.

- **Know a useful fork?** Open an issue in the relevant repository with a link and a short note on what it adds.
- **Porting a change?** Keep each pull request focused, link the source fork and commit, and credit the original author with a `Co-authored-by:` trailer.
- **Commit messages:** follow the conventions in [AGENTS.md](https://github.com/ha-c4/.github/blob/main/AGENTS.md).

## Disclaimer

ha-c4 is an independent, community-maintained project. It is **not** affiliated with, endorsed by, sponsored by, or supported by the Home Assistant project, Nabu Casa, Control4, Snap One, or any of their affiliates.

Home Assistant, Control4, and all other product names and trademarks mentioned here belong to their respective owners. They are used only to describe compatibility.

This software comes with no warranty. Use it at your own risk. For official support of your Control4 system, contact your Control4 dealer.
