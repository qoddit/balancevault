# Project Overview

**Balance** is a C terminal chat application using a curses-style text interface and CMake-based build. The project goals documented in conversation include local accounts, encrypted communications and storage, friend/tunnel requests, file transfer, optional cloud sync, and a low-distraction TUI.

## Design goals
- Terminal-first interface with chat content scrolling and a persistent prompt.
- Explicit commands using `?` (for example, `?clear`) and `-h` for help.
- Encryption before transmission or cloud storage; no plaintext credentials.
- Volatile sessions should not be written into persistent chat history.
- Optional cloud backends should not be required for basic local/volatile operation.
- No telemetry, tracking, or unnecessary logging.

## Related notes
- [[Architecture Map]]
- [[Security Model]]
- [[TUI and Input]]
- [[Networking and Protocol]]
- [[Storage and Chat History]]
- [[File Transfer]]
- [[Cloud Backends]]

> These are project goals/context, not a claim that every feature is fully implemented or verified in every source snapshot.
