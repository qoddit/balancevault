# Balance — Obsidian project map

> A linked knowledge map for the Balance project. Notes describe the repository snapshot used to make this vault; they are documentation notes, not a replacement for source code.

## Start here
- [[Project Overview]] — purpose, scope, and constraints
- [[Architecture Map]] — major modules and their connections
- [[Repository File Index]] — every repository file represented by a note
- [[Build and Development]] — build requirements and workflow
- [[Security Model]] — security goals and boundaries
- [[TUI and Input]] — curses UI, commands, and scrolling
- [[Networking and Protocol]] — peer communication and message protocol
- [[Storage and Chat History]] — local persistence
- [[Cloud Backends]] — optional cloud integration
- [[Testing and Release]] — tests, CI, packaging

## Key relationships
[[main.c]] starts the program and coordinates [[ui.c]], [[commands.c]], and shared facilities. [[ui.c]] depends on [[commands.c]] and [[common.c]]; [[net.c]] and [[proto.c]] implement communication; [[crypto.c]] supplies cryptographic operations; [[store.c]] handles persistence; [[cloud.c]] contains optional cloud-backend integration.

## Snapshot caveat
The available source archive is named `balance-beta-0.3.4-mouse-scroll-20261007.zip`, while its internal top-level directory says `balance-beta-0.3.3-curses-scroll-20261007`. The included `VERSION`/CMake metadata should be checked against the actual working Git repository before treating this map as authoritative for a newer checkout. See [[Repository File Index]].
