# counterread

A desktop markdown editor where an AI expert panel argues with your draft, the criticism is
stored **inside the markdown file** for your coding agent to read, and every revision is a git
commit.

> Essays, reviewed by a panel, edited with Claude.

**[Product page →](https://a7medkamel.github.io/counterread/)**
· **[Download for macOS →](https://github.com/a7medkamel/counterread/releases/latest)**

This repository hosts the product page and the signed macOS downloads.

## What it does

- **An adversarial review panel.** Seven personas designed for your specific document —
  operator, thought leader, investor, academic, practitioner, plus wildcards — debate your
  most contestable passages in parallel, each a separate agent with its own system prompt and
  optionally its own model. A moderator closes each thread with a verdict and one concrete
  edit.
- **Comments stored in the file.** Everything is written as
  [CriticMarkup](https://github.com/CriticMarkup/CriticMarkup-toolkit) inside the markdown, so
  Claude Code reads the feedback in place and revises the document. The editor watches the
  file and reloads when it changes on disk.
- **Read aloud, talk back.** Read mode reads the document in a neural voice and keeps the mic
  live — speak and your objection is transcribed and anchored to the sentence being read.
  Speech synthesis and transcription both run on-device.
- **Git-backed revisions.** Autosave, auto-commit on idle, history with provenance, diff and
  restore.

## Install

Download the `.dmg` from [Releases](https://github.com/a7medkamel/counterread/releases/latest),
open it, and drag counterread to Applications.

Builds are signed and notarized with Apple, so they open normally.

New versions download in the background and install when you quit.

Requires macOS on Apple Silicon and `git`. The review panel needs your own
[OpenRouter](https://openrouter.ai) API key; the voice features need nothing.

## License

MIT
