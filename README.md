# bunbot

[![npm (tag)](https://img.shields.io/npm/v/bunbot?style=flat&colorA=000000&colorB=000000)](https://www.npmjs.com/package/bunbot) ![NPM](https://img.shields.io/npm/l/bunbot?style=flat&colorA=000000&colorB=000000)

<p align="center">
  <img src="https://i.imgur.com/iQgEyms.jpg">
</p>
<p align="center">
  Generated using <a href="https://www.craiyon.com">Craiyon</a>.
</p>

Native cross-platform GUI automation for the Bun runtime. Supports Mac and Windows for now.

## Requirements

Bunbot uses [RobotGo](https://github.com/go-vgo/robotgo) via `bun:ffi`. Please see RobotGo's requirements [here](https://github.com/go-vgo/robotgo#requirements).

## Usage

```bash
bun add bunbot
```

### Mouse

```ts
import Bunbot from 'bunbot'

const bb = new Bunbot()

// Click
bb.click()
// Get mouse position coordinates
const mousePosition = bb.getMousePosition()
// Move mouse
bb.moveMouse(200, 400)
// Move mouse smoothly
bb.moveMouseSmooth(200, 400)
// Scroll mouse
bb.scrollMouse(100, 200)
```

### Keyboard

```ts
import Bunbot from 'bunbot'

const bb = new Bunbot()

// Type a string
bb.type('Hello world!')
// Tap a key
bb.tap('i', 'alt', 'command')
```

### Screen

```ts
import Bunbot from 'bunbot'

const bb = new Bunbot()

// Get screen size
const screenSize = bb.getScreenSize()
// Get mouse pos's color
const color = bb.getMousePositionColor()
// Get scale size
const scaleSize = bb.getScaleSize()
```

More functions to come...

## Development

[View instructions](/Development.md)

## License

MIT
