<img src="" />

<p align="center">Tonecard is one of the best canvas libraries to create a variety of music cards.</p>

<p align="center">
    <a href=""><b>Github</b></a> •
    <a href="https://dsc.gg/discronix"><b>Support</b></a>
</p>

<div align="center">

[![NPM Version](https://img.shields.io/npm/v/musicard?style=flat-square&color=%23FF7A00)](https://www.npmjs.com/package/musicard)
[![NPM Downloads](https://img.shields.io/npm/dw/musicard?style=flat-square&color=%23FF7A00)](https://www.npmjs.com/package/musicard)
[![NPM License](https://img.shields.io/npm/l/musicard?style=flat-square&color=%23FF7A00)](https://github.com/unburn/musicard/blob/main/LICENSE)
[![GitHub Repo stars](https://img.shields.io/github/stars/unburn/musicard?style=flat-square&color=%23FF7A00)](https://github.com/unburn/musicard)

</div>

<div align="center">
<a href="https://github.com/discronix/Tonecard/"><img src="https://ik.imagekit.io/unburn/SupportMusicard.svg"/></a>
</div>

# Installation
```js
// using npm
npm install Tonecard

// using yarn
yarn add Tonecard
```

# Usage
You can use the Tonecard package in your Discord bots, websites, etc.

## Using Create File
```js
import { Classic } from "Tonecard";
import fs from 'fs'

//OR

const { Classic } = require("Tonecard");
const fs = require('fs')

Classic({}).then(x => {
    fs.writeFileSync("output.png", x)
})
```

## Using Discord Bot
```js
const { Classic } = require("Tonecard");
const fs = require("fs")

const Tonecard = await Classic({});

...

return message.channel.send({
    files: [{
        attachment: Tonecard
    }]
})
```

## Custom Background (New)
Use a custom image background and also adjust the darkness of the image.
```js
import { Classic } from "Tonecard";
import fs from 'fs'

Classic({
    thumbnailImage: "https://cdn.discordapp.com/attachments/1220001571228880917/1220001571690123284/01.png?ex=660d5a01&is=65fae501&hm=a8cfb44844e61aa0fd01767cd363af048df28966c30d7b04a59f27fa45cf69c4&",
    backgroundImage: "https://cdn.discordapp.com/attachments/1220001571228880917/1220001571690123284/01.png?ex=660d5a01&is=65fae501&hm=a8cfb44844e61aa0fd01767cd363af048df28966c30d7b04a59f27fa45cf69c4&",
    imageDarkness: 60,
    nameColor: "#DC92FF",
    progressColor: "#DC92FF",
    progressBarColor: "#2B2B2B",
    progress: 50
}).then(x => {
    fs.writeFileSync("output.png", x)
})
```

![custom](https://ik.imagekit.io/unburn/custom-output.png?updatedAt=1710995171966)

# Themes
Tonecard is the #1 canvas library to create music cards with awesome themes.

## Classic

![classic](https://ik.imagekit.io/unburn/Classic.svg)

```js
(async () => {
    const { Classic } = require("Tonecard");
    const fs = require("fs")

    const Tonecard = await Classic({
        thumbnailImage: "https://lh3.googleusercontent.com/yavtBZZnoxaY21GSS_VIKSg0mvzu1b0r6arH8xvWVskoMaZ5ww3iDMgBNujnIWCt7MOkDsrKapSGCfc=w544-h544-l90-rj",
        backgroundColor: "#070707",
        progress: 10,
        progressColor: "#FF7A00",
        progressBarColor: "#5F2D00",
        name: "Burn",
        nameColor: "#FF7A00",
        author: "By 2WEI & Edda Hayes",
        authorColor: "#696969",
        startTime: "0:00",
        endTime: "4:00",
        timeColor: "#FF7A00"
    });

    fs.writeFileSync("Tonecard.png", Tonecard);
})()
```

***

## Classic Pro

![classicpro](https://ik.imagekit.io/unburn/ClassicPro.svg)

```js
(async () => {
    const { ClassicPro } = require("Tonecard");
    const fs = require("fs")

    const Tonecard = await ClassicPro({
        thumbnailImage: "https://lh3.googleusercontent.com/yavtBZZnoxaY21GSS_VIKSg0mvzu1b0r6arH8xvWVskoMaZ5ww3iDMgBNujnIWCt7MOkDsrKapSGCfc=w544-h544-l90-rj",
        backgroundColor: "#070707",
        progress: 10,
        progressColor: "#FF7A00",
        progressBarColor: "#5F2D00",
        name: "Burn",
        nameColor: "#FF7A00",
        author: "By 2WEI & Edda Hayes",
        authorColor: "#696969",
        startTime: "0:00",
        endTime: "4:00",
        timeColor: "#FF7A00"
    });

    fs.writeFileSync("Tonecard.png",Tonecard);
})()
```

***

## Dynamic

![dynamic](https://ik.imagekit.io/unburn/Dynamic.svg)

```js
(async () => {
    const { Dynamic } = require("Tonecard");
    const fs = require("fs")

    const Tonecard = await Dynamic({
        thumbnailImage: "https://lh3.googleusercontent.com/yavtBZZnoxaY21GSS_VIKSg0mvzu1b0r6arH8xvWVskoMaZ5ww3iDMgBNujnIWCt7MOkDsrKapSGCfc=w544-h544-l90-rj",
        backgroundColor: "#070707",
        progress: 10,
        progressColor: "#FF7A00",
        progressBarColor: "#5F2D00",
        name: "Burn",
        nameColor: "#FF7A00",
        author: "By 2WEI & Edda Hayes",
        authorColor: "#696969"
    });

    fs.writeFileSync("Tonecard.png", Tonecard);
})()
```

***

## Mini

![mini](https://ik.imagekit.io/unburn/Mini.svg)

```js
(async () => {
    const { Mini } = require("Tonecard");
    const fs = require("fs")

    const Tonecard = await Mini({
        thumbnailImage: "https://lh3.googleusercontent.com/yavtBZZnoxaY21GSS_VIKSg0mvzu1b0r6arH8xvWVskoMaZ5ww3iDMgBNujnIWCt7MOkDsrKapSGCfc=w544-h544-l90-rj",
        backgroundColor: "#070707",
        progress: 10,
        progressColor: "#FF7A00",
        progressBarColor: "#5F2D00",
        menuColor: "#FF7A00",
        paused: false
    });

    fs.writeFileSync("Tonecard.png", Tonecard);
})()
```

# Resource
Pull request to add your project here.

|  |  |
| --------------- | --------------------------------------------- |

# Licence
[GPL](https://github.com/discronix/Tonecard/blob/main/LICENSE)
