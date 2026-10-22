# File Transfer

Project requirements describe request-based peer-to-peer file transfer, a destination shaped like `transfers/<chat_name>`, an actionable request pinned near the prompt, a click action that fills the command into the prompt, and progress/speed/percentage display.

Relevant modules to inspect: [[ui.c]] for presentation and input, [[commands.c]] for request actions, [[net.c]] / [[proto.c]] for transport, and [[crypto.c]] for protected transfer content.

Implementation status must be confirmed in the checked-out source; this note records the target behavior rather than asserting complete support.
