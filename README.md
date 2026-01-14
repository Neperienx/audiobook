# KidBook Audiobook Builder (PoC)

A tiny Python pipeline to turn a page-based kids story into per-page audio files (and optionally a single combined audiobook).
Designed so you can start with the OpenAI Text-to-Speech API, then later swap in a local TTS backend.

## Goals

- **Input format:** JSON story with `page_number` + `text`
- **Optional narration overrides:** a separate file you can edit without touching story structure
- **Output:** one audio file per page (e.g., `001.mp3`, `002.mp3`, ...) and a manifest
- **Swappable TTS backends:** `openai` now, `local` later

---

## Project structure

