# RK Workspace

The desktop app for [RK](https://github.com/rk-platform/core), the Research Knowledge
Platform, a local-first workspace built around AI. It brings your AI models, documents, notes
and the web into one environment: it shows an RK project's files and runs RK's commands from a
command palette (⌘K), talking to the same background daemon (RK Core) as the `rk` command line.

This repository holds the app's releases. RK itself, and the installer that sets up both,
live in [rk-platform/core](https://github.com/rk-platform/core).

RK is about to go into alpha testing, 

RK Workspace runs on Apple Silicon Macs, with support for Windows and Linux comming soon.

## Requirements

- An Apple Silicon Mac with macOS 15 or later.
- RK itself. The app starts RK's daemon when it needs one, and cannot work without it.

## Install

Installing RK installs the app into `/Applications` as part of its own setup:

    curl -fsSL https://raw.githubusercontent.com/rk-platform/core/HEAD/install.sh | sh

Then open the app from Launchpad or Spotlight. The daemon will be started automatically.

## Update

    rk update

updates RK and, when a newer app has been released here, the app as well. The two are released
separately: the app asks the daemon it connects to which commands it has, so a newer RK does
not need a newer app. [CHANGELOG.md](CHANGELOG.md) lists what changed in each release.

## License

RK Workspace is proprietary software, under the same end user license agreement as RK. See [LICENSE](LICENSE).
