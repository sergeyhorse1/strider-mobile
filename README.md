# Strider — mobile habit tracker

> Native mobile habit tracker focused on animation polish: swipeable cards, Skia-based custom charts, full haptic feedback, Reanimated 3 worklets. Built with Expo SDK 52+.

[![CI](https://github.com/sergeyhorse1/strider-mobile/actions/workflows/ci.yml/badge.svg)](https://github.com/sergeyhorse1/strider-mobile/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Status](https://img.shields.io/badge/status-in_development-orange)

🚧 **Status:** in active development. APK and screenshots will appear here as features land.

---

## EN

### What it is
A native mobile habit tracker (Android, iOS-ready) targeting Things 3 / Streaks / Reflect levels of UX polish: Tinder-style swipe-to-complete cards, Skia-based animated streak flame and yearly heatmap, custom blurred tab bar, haptics on key actions, scheduled notifications, dark/light theme. Built to demonstrate Expo + Reanimated 3 + Skia + Drizzle expertise.

### Stack
Expo SDK 52+ (Expo Router, Expo Notifications, Expo Haptics) · React Native 0.76+ · TypeScript (strict) · Reanimated 3 + Gesture Handler · React Native Skia · NativeWind · Zustand + Immer · Drizzle ORM + expo-sqlite · date-fns · Jest + React Native Testing Library · Maestro

### Highlights
- Reanimated 3 worklets for 60fps gesture-driven UI (drag/swipe/spring)
- Skia animated streak flame (shader-driven) and yearly heatmap
- Typed local DB via Drizzle + SQLite (no remote backend)
- Expo development build (not Expo Go) — required for Skia + Reanimated 3 native modules
- Haptics on every meaningful interaction (gesture, success, toggle)
- `react-native-reanimated/plugin` always last in `babel.config.js`

### Run locally
```bash
pnpm install
pnpm expo prebuild
pnpm expo run:android       # development build on Android emulator/device
```

> Requires Android Studio + an emulator (or a connected device). iOS build needs Xcode and isn't the primary target.

---

## RU

### Что это
Нативное мобильное приложение трекера привычек (Android, готово к iOS) с целевым уровнем полировки Things 3 / Streaks / Reflect: свайп-карточки в стиле Tinder, Skia-анимации (огонёк streak, годовой heatmap), кастомный blur tab bar, хаптика, локальные уведомления, тёмная/светлая темы. Демонстрация Expo + Reanimated 3 + Skia + Drizzle.

### Стек
Expo SDK 52+ (Expo Router, Expo Notifications, Expo Haptics) · React Native 0.76+ · TypeScript (strict) · Reanimated 3 + Gesture Handler · React Native Skia · NativeWind · Zustand + Immer · Drizzle ORM + expo-sqlite · date-fns · Jest + RN Testing Library · Maestro

### Highlights
- Reanimated 3 worklet'ы для 60fps жестов (drag/swipe/spring)
- Skia: анимированный огонёк streak (на шейдерах) и годовой heatmap
- Типизированная локальная БД через Drizzle + SQLite (без бэкенда)
- Expo development build (не Expo Go) — нужны нативные модули Skia + Reanimated 3
- Хаптика на каждом значимом взаимодействии (жест, success, toggle)
- `react-native-reanimated/plugin` всегда последним в `babel.config.js`

### Запуск локально
```bash
pnpm install
pnpm expo prebuild
pnpm expo run:android
```

> Нужен Android Studio + эмулятор или физическое устройство. iOS — не основная цель.

---

## License
[MIT](LICENSE)
