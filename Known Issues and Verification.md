# Known Issues and Verification

## Source archive naming mismatch
The source archive used to create this vault has a filename indicating beta-0.3.4, but its root directory is named beta-0.3.3. Treat the checked-out Git repository as authoritative and verify `VERSION`, `CMakeLists.txt`, and `src/version.h` agree.

## Mouse/trackpad scrolling
A previous report says trackpad scrolling did not work in the user's terminal. Do not mark this fixed solely because mouse-wheel code exists. Verify behavior in the target terminal emulator on macOS.

## Build verification
Do not claim a build or tests passed without running them against the current checkout. Clean stale build directories when switching OS/architecture. See [[Testing and Release]].
