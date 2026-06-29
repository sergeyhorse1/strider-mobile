# Strider — voice second brain

> Tap, talk for 10 seconds, find it back later by searching. Privacy-first: nothing leaves your phone.

[![CI](https://github.com/sergeyhorse1/strider-mobile/actions/workflows/ci.yml/badge.svg)](https://github.com/sergeyhorse1/strider-mobile/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Status](https://img.shields.io/badge/status-in_development-orange)

🚧 **Status:** in active development. APK and screenshots will appear here.

---

## EN

### What it is
Native mobile app for capturing thoughts by voice. Hold a button, speak for a few seconds (an idea, a reminder, a note about someone), release. On-device Whisper transcribes the audio, simple cleanup heuristics polish the result, full-text search finds it back later. Nothing leaves your phone — privacy by design.

### Stack
Expo SDK (latest) · React Native (latest) · TypeScript (strict) · Reanimated 4 + Gesture Handler · React Native Skia (audio waveform) · NativeWind + Tailwind · Zustand + Immer · Drizzle ORM + expo-sqlite (with FTS5) · expo-audio · whisper.rn (on-device transcription) · date-fns + date-fns-tz · Jest + React Native Testing Library · Maestro (e2e) · EAS Build

### Highlights
- Fully on-device: Whisper runs locally, audio never leaves the phone
- Hold-to-record with Skia-driven waveform feedback
- Full-text search via SQLite FTS5 across all transcripts (Cyrillic + Latin)
- Cleanup heuristics remove fillers ("uh", "um"), capitalize sentences
- 60fps gesture-driven UI on Reanimated 4 worklets

### Run locally
```bash
pnpm install
pnpm expo prebuild
pnpm expo run:android   # development build (Expo Go won't work — needs native modules)
```

> Requires Android Studio + emulator/device. iOS build needs Xcode.

---

## RU

### Что это
Нативное мобильное приложение для записи мыслей голосом. Зажимаешь кнопку, говоришь несколько секунд (идея, напоминание, заметка о ком-то), отпускаешь. On-device Whisper транскрибирует звук, эвристики причёсывают текст, full-text search находит позже по нескольким словам. Ничего не уходит в интернет — приватность из коробки.

### Стек
Expo SDK (latest) · React Native (latest) · TypeScript (strict) · Reanimated 4 + Gesture Handler · React Native Skia (waveform) · NativeWind + Tailwind · Zustand + Immer · Drizzle ORM + expo-sqlite (с FTS5) · expo-audio · whisper.rn (on-device транскрипция) · date-fns + date-fns-tz · Jest + RNTL · Maestro · EAS Build

### Highlights
- Полностью on-device: Whisper работает локально, аудио никуда не уходит
- Hold-to-record с Skia-визуализацией waveform'ы
- Full-text поиск через SQLite FTS5 по всем транскриптам (кириллица + латиница)
- Эвристики чистки убирают «эээ», «ммм», капитализируют предложения
- 60fps жесты на Reanimated 4 worklet'ах

### Запуск локально
```bash
pnpm install
pnpm expo prebuild
pnpm expo run:android       # development build (Expo Go не подойдёт — нужны нативные модули)
```

> Нужен Android Studio + эмулятор/устройство. iOS — Xcode.

---

## License
[MIT](LICENSE)
