# chrome-tab-react

Scaffold a Chrome Extension with React

## Setup

- Install react typescript

```shell
yarn create react-app <name> --template typescript
```

- Create `manifest.json` in root folder to run Chrome extension

```json
{
  "manifest_version": 2,

  "name": "My Extension",
  "description": "This extension is a starting point to create a real Chrome extension",
  "version": "0.0.1",

  "browser_action": {
    "default_popup": "index.html",
    "default_title": "Open the popup"
  },
  "icons": {
    "16": "logo-small.png",
    "48": "logo-small.png",
    "128": "logo-small.png"
  },
  "permissions": []
}
```

> `browser_action` section tells Chrome that we will have a popup which will run the `index.html`

## Deploy

- Build project

```
yarn run build
```

- Add extension by navigating to

```
chrome://extensions/
```

- Load unpacked extension
- Go to the build folder and press OK
