# TGCallsJs [![More in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)

An operative library for Telegram calls and a tgcalls helper.

## Features

-   Super light & easy-to-use.
-   Smart stream function.
-   Smartest streamAudio function.
-   Native controls: pause, resume, mute, unmute.
-   Call helpers: join, edit, leave.

## Installation

```shell
npm i tgcallsjs
```

## Example usage with audio

First install ffmpeg in your system otherwise it will generate errors  

## For windows:  
download this and set its path in environment variable  
https:telegram.me/logicbots/180  

## for ubuntu:
sudo apt install ffmpeg  

like this you can install on other os  

```js
const { TGCallsJs, gramjs } = require("tgcallsjs");

// Replace these values with actual values
const apiId = 123456;
const apiHash = "392ykiyourhashhere";
const stringSession = "";

(async () => {
 const client = await gramjs(apiId, apiHash, stringSession);
  console.log(client.session.save()); // use this value in stringSession after 1 time generate
  let tg = new TGCallsJs(client, "groupusername");
  tg.streamAudio("./audio.mp3");
})();

```

## Docs

The docs can be found [here](https://tgcallsjs.github.io/gram-tgcalls).  

## Credits

-   Structure inspired from Telethon bridge in [MarshalX/tgcalls](https://github.com/MarshalX/tgcalls).  
-   Video support by [@Laky-64](https://github.com/Laky-64).  
-   Latest version with easiness by [@PanditSiddharth](https://telegram.me/panditSiddharth)  

inherited: tgcalls -> gram-tgcalls -> tgcallsjs

