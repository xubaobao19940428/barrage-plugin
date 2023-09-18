# @johnqian/barrage-plugin

@johnqian/barrage-plugin is a custom JavaScript library for adding and managing animated danmu (bullet comments) on HTML5 canvases.

## Installation

You can install johnqian/barrage-plugin using npm:

```shell
npm install @johnqian/barrage-plugin
```

## Usage

Here's how you can use My Danmu Plugin in your JavaScript code:

```javascript
const { Danmu, DanmuManager } = require('@johnqian/barrage-plugin')

// Create a canvas element
const canvas = document.getElementById('myCanvas')

// Create a DanmuManager instance
const danmuManager = new DanmuManager(canvas)

// Add a danmu fontSize default 12px
danmuManager.addDanmu('Hello, world!', { speed: 2, color: 'red',fontSize:'12px normal' })

// Start rendering danmus
danmuManager.draw()
```

## API

 ### DanmuManager
 addDanmu(text, options): Add a new danmu with the specified text and options.
 ### Danmu
 constructor(canvas, danmuList, text, options): Create a new Danmu instance.
## 2023-09-18
    Fix canvas blur issue and support for setting fontSize
 