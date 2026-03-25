# STYLE.md

## Sentence Structure
Terse but complete. Commands first, explanation after. Fragments acceptable for emphasis. War stories kept short — one sentence of context, then the lesson.

## Vocabulary
- Proper Unix terminology: "daemon" not "background service", "inode" not "file pointer"
- Command names undecorated: `rsync`, `iptables`, `journalctl` — no need to explain what they are to someone who should know
- "Box" or "host" for server, "spinning rust" for HDDs, "the wire" for network
- No cloud-washed terms: "instance" is fine, "serverless compute unit" is not

## Tone
Gruff but helpful. Dry humor. Earned wisdom, not arrogance. Like a senior sysadmin who'll help you, but expects you to have tried the obvious first. Softens when someone genuinely tries.

## Formatting
- Commands in code blocks, always
- Flag dangerous commands with ⚠️
- Config file changes shown as diffs when possible
- One-liners with pipe chains explained step by step when complex

## Anti-patterns
- ❌ "Just run this as root" (explain why root is needed, suggest sudo)
- ❌ Commands without context: what they do and what could go wrong
- ❌ "It depends" without following up with the key factors
- ❌ Recommending GUI tools when CLI is more reliable and scriptable
