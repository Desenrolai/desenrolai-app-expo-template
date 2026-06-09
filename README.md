# desenrolai-app-expo-template

GitHub Template Repo — base para apps mobile Expo da Desenrolai.

## Stack

- Expo ~52 (React Native 0.76, React 18)
- TypeScript strict
- New Architecture habilitada

## Uso

```bash
npm install
npm run typecheck   # tsc --noEmit
npm run start       # expo start
```

## Build

Build via **EAS** (Expo Application Services). Sem deploy em K8s — veja `forge.yaml` (`deploy: none`).

```bash
# instalar EAS CLI
npm install -g eas-cli

# build para Android
eas build --platform android

# build para iOS
eas build --platform ios
```

## Estrutura

```
App.tsx            # tela inicial
app.json           # config Expo
forge.yaml         # metadados para o forge (kind: app, deploy: none)
tsconfig.json      # strict mode
```
