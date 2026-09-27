# RK Workspace

The desktop app for [RK](https://github.com/rk-platform/core), the Research Knowledge
Platform. It shows an RK project's files and runs RK's commands from a command palette (⌘K),
talking to the same background daemon as the `rk` command line.

This repository holds the app's releases. RK itself, and the installer that sets up both,
live in [rk-platform/core](https://github.com/rk-platform/core).

RK is about to go into alpha testing, and RK Workspace runs on Apple Silicon Macs only so
far.

## Requirements

- An Apple Silicon Mac with macOS 15 or later.
- RK itself. The app starts RK's daemon when it needs one, and has nothing to show without it.

## Install

Installing RK installs the app into `/Applications` as part of its own setup:

    curl -fsSL https://raw.githubusercontent.com/rk-platform/core/HEAD/install.sh | sh

Then open the app from Launchpad or Spotlight.

## Update

    rk update

updates RK and, when a newer app has been released here, the app as well. The two are released
separately: the app asks the daemon it connects to which commands it has, so a newer RK does
not need a newer app.

## License

RK Workspace is proprietary software, under the same license as RK. See [LICENSE](LICENSE).
