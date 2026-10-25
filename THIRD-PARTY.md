# Third-party code

This project is a derivative work combining pieces of two other MIT-licensed
projects. Both license texts are reproduced in full below, as MIT requires.

## TWBankston/Seeker-TV-Launcher

`launcher/index.html`'s 5x7 dot-matrix font and icon set, the wheel layout math,
the clock/weather panel layout, the cursor glow, the launch-takeover animation,
and the remote-key handling (Up/Down/Enter/Back) are ported from the WHEEL home
screen mockup in [TWBankston/Seeker-TV-Launcher](https://github.com/TWBankston/Seeker-TV-Launcher)
(`design/seeker-tv-mockup-v3.html`), adapted from a standalone browser mockup to
run as a webOS app talking to CleanYourTV's local API instead of Android intents.

```
MIT License

Copyright (c) 2026 TWBankston

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## lasharor/cleanyourtv-WebOS

`launcher/index.html`'s per-app colour extraction (`iconColor`, `analyse`,
`rgb2hsl`, `hsl2rgb`, `hashHue`) is ported from
[lasharor/cleanyourtv-WebOS](https://github.com/lasharor/cleanyourtv-WebOS)'s
stock `app/index.html`, so app colours match the rest of the system. The files
in `patches/` are CleanYourTV's own `helper/config.js` and `helper/apps.js`,
each with one small addition (see the comments marked "Not part of upstream
CleanYourTV" in each file) to let a custom launcher persist a full app order
and per-app renamed labels, which CleanYourTV's own config schema doesn't have
room for. This project would not exist without CleanYourTV, which this launcher
runs as a drop-in replacement for `app/index.html` inside.

```
MIT License

Copyright (c) 2026 cleanyourtv-WebOS contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
