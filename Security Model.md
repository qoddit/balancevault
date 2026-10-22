# Security Model

## Intended properties
- Credentials should not be stored as plaintext.
- Messages should be encrypted before network transmission and before cloud persistence.
- Volatile conversations should remain out of persistent local chat history.
- No telemetry, tracking, or sensitive plaintext logs.
- Optional cloud sync should preserve end-to-end encryption (E2EE) boundaries.

## Review questions
1. Where are keys derived, stored, and cleared? See [[crypto.c]] and [[crypto.h]].
2. Which data reaches disk? See [[store.c]] and [[Storage and Chat History]].
3. What leaves the machine? See [[net.c]], [[proto.c]], and [[Cloud Backends]].
4. Are error paths and debug output free of secrets?
5. Are nonce, salt, KDF, authentication, and versioning choices documented and tested?

## Important distinction
These are project requirements and review prompts, not an independent security audit. Read [[SECURITY.md]] and the current source before making security claims.
