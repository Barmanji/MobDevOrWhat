# First Mob-App

A dark-themed task management app built with Expo, React Native, and TypeScript. Browse, filter, and track your daily tasks with a clean, modern UI.
<img width="1240" height="2772" alt="Screenshot_2026-05-24-19-50-00-97_f73b71075b1de7323614b647fe394240 jpg" src="https://github.com/user-attachments/assets/7a98d876-d55c-40ae-9eac-7d813980d755" />

## Features

- **Task List** — Scrollable list of tasks with status, category, time, and icon
- **Date Selector** — Horizontal date picker to switch between days
- **Filter Tabs** — Filter tasks by All, To Do, In Progress, or Completed
- **Status Indicators** — Color-coded badges (Done / In Prog / To-do)
- **Dark Theme** — Amber-gold accent on a rich dark background

## Tech Stack

- [Expo](https://expo.dev) (SDK 56) with Expo Router
- React Native (0.85) + TypeScript
- `@expo/vector-icons` (Ionicons)
- `expo-router` (file-based routing)
- `react-native-safe-area-context`
- `react-native-gesture-handler` & `react-native-reanimated`

## Getting Started

```bash
npm install
npx expo start
```
> Make sure the dev mode is on, on mobile. And USB-Debugging is On.

Then open the app in:
- [Expo Go](https://expo.dev/go) (scan QR code)
- Android emulator (`npx expo start --android`)
- iOS simulator (`npx expo start --ios`)
- Web browser (`npx expo start --web`)

## Project Structure

```
src/
├── app/
│   ├── _layout.tsx      # Root layout (header hidden)
│   └── index.tsx        # Home screen with FlatList
├── components/
│   ├── Header.tsx        # "Today's Task" title + back/notif buttons
│   ├── DateSelector.tsx  # Horizontal date picker
│   ├── FilterTabs.tsx    # All / To do / In Prog / Completed tabs
│   └── TaskCard.tsx      # Individual task card
├── constants/
│   ├── Colors.ts         # Dark theme color palette
│   └── Tasks.ts          # Task types, mock data, filter options
```

## Scripts

| Command           | Description          |
| ----------------- | -------------------- |
| `npm start`       | Start Expo dev server |
| `npm run android` | Start on Android      |
| `npm run ios`     | Start on iOS          |
| `npm run web`     | Start on web          |
| `npm run lint`    | Run ESLint            |

## License

MIT
