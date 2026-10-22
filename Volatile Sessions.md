# Volatile Sessions

A volatile session is intended to exist only while participants are connected and should not be written to local chat history or cloud storage. This concept touches [[Networking and Protocol]], [[Storage and Chat History]], [[Security Model]], and [[TUI and Input]].

Questions to verify: what happens on disconnect, whether buffers are cleared, whether reconnect is possible, and whether any crash/debug path writes message content.
