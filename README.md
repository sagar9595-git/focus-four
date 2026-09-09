# Focus Four

A minimal Eisenhower Matrix task manager built as a single static HTML page.

## Features

- Four urgency and importance quadrants
- Optional target dates
- Strike-through or remove-on-complete modes
- Local browser persistence
- Optional private OneDrive sync through Microsoft Graph
- Responsive desktop and mobile layout

## Run locally

```powershell
npx --yes http-server . -p 5500 -c-1
```

Open `http://localhost:5500/`.

## OneDrive sync

1. Register a single-page application in Microsoft Entra.
2. Add the redirect URI displayed in the app's Settings panel.
3. Grant the delegated `Files.ReadWrite.AppFolder` Microsoft Graph permission.
4. Enter the application client ID in Settings, then select the cloud button.

Tasks are stored in OneDrive's private application folder as `focus-four.json`.
