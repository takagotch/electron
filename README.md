### electron
---
https://electronjs.org/

https://github.com/electron/electron

https://electronjs.org/docs/api

```
npm install electron --save-dev [--save-exact]
npm install
npm start

npm i -D electron@latest
npm i -D electron@beta
npm i -D electron-nightly
```

```js
const electron = require('electron')
const proc = require('child_process')

console.log(electron)

const child = proc.spawn(electron)
```

```js
const { app, globalShortcut } = require('electron')

app.on('ready', () => {
  globalShorcut.register('CommandorControl+Y', () => {
  })
})

const { app } = require('electron')
app.on('window-all-closed', () => {
  app.quit()
})

const { app } = require('electron')

app.relaunch({ args: process.argv.slice(1).concat(['--relaunch'])})
app.exit(0)

```
