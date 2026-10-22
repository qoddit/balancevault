# Cloud Backends

[[cloud.c]] / [[cloud.h]] contain cloud-related functionality in this repository snapshot. The project direction discussed includes optional Supabase, Google Drive, and self-hosted storage, with E2EE before cloud persistence and possible migration from a volatile session.

Cloud should be optional and should not be confused with the peer/volatile transport path. Check the current source and configuration before assuming each named provider is implemented.

Related: [[Security Model]], [[crypto.c]], [[store.c]], [[net.c]].
