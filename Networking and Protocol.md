# Networking and Protocol

[[net.c]] / [[net.h]] provide network operations; [[proto.c]] / [[proto.h]] define protocol-level helpers; [[crypto.c]] provides cryptographic functions used around data exchange. [[server.c]] contains server/listener functionality in this snapshot.

## Review flow
1. Identify the call path from [[commands.c]] to [[net.c]].
2. Confirm message framing and validation in [[proto.c]].
3. Confirm encryption/authentication boundaries in [[crypto.c]].
4. Confirm timeouts, disconnects, and rejected-request cleanup.

Related concepts: [[Security Model]], [[File Transfer]], [[Cloud Backends]].
