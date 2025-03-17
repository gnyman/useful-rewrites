# useful-rewrites
A small collection of useful rewrites to make the web experience less bad.

If you are looking for something that helps you access twitter/instagram/etc I recommend looking at [libredirect](https://libredirect.github.io/). This list is mostly for fixing annoyances.

## how do I use these?
### Safari iOS and Firefox / Chrome / Chromium browsers on Mac 
[StopTheMadness Pro](https://apps.apple.com/app/stopthemadness-pro/id6471380298)  
Note: StopTheMadness Pro does a lot of other quality-of-life improvements but if you are just looking for a redirector maybe Redirector is better.

### Chrome / Firefox / Edge / Opera / Chromium on any OS
[Redirector](https://einaregilsson.com/redirector/)

## Rewrites
### Zoom: Skip directly to meeet in browser
This skips the landing page which will auto-download the zoom installer and goes directly to the corresponding link for joining with browser.

`/https:\/\/(?:.*?)zoom\.us\/j\/(\d+)(\?pwd=([^&\s"')]+))?/` ⮕ `https://app.zoom.us/wc/$1/join?fromPWA=1&pwd=$3`

### Webex: Skip the landing page and join meeting with the browser

`/(https:\/\/.*\.webex\.com\/meet\/[^?#]+)($|[?#])/` ⮕ `$1?launchApp=true$2`
