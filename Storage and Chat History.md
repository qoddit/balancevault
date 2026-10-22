# Storage and Chat History

[[store.c]] / [[store.h]] are the local persistence module. They should be reviewed alongside [[crypto.c]] for encryption behavior and [[commands.c]] for the paths that invoke storage.

## Required behavior
- Logged-in users may have local encrypted chat history.
- Volatile chats should not touch persistent history.
- Credentials and private key material must not be written in plaintext.
- Runtime files and vault data should not accidentally enter Git.

See [[Security Model]], [[.gitignore]], and [[Known Issues and Verification]].
