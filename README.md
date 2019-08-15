# Pocket Bar

A simple plugin to [BitBar](https://getbitbar.com/) as the basic [Pocket](https://getpocket.com/) client working in your Mac menu bar.

![](https://i.imgur.com/XQnh7US.png)

Supports main actions: retrieve articles, add or delete (use ⌥) an article.

![](https://i.imgur.com/I7BVKcD.png)

## Instructions

1. Install the latest version of [BitBar](https://github.com/matryer/bitbar/releases/latest). I recommend to use [Homebrew](https://brew.sh/): run `brew cask install bitbar` in the terminal window.
2. Install [Python 3](https://python.org), [pocket-api](https://github.com/rakanalh/pocket-api) and [keyring](https://github.com/jaraco/keyring) packages: `brew install python && pip3 install -U pocket-api keyring`.
3. Copy [pocket.10m.py](pocket.10m.py) to your BitBar plugins folder (e.g. with curl), and run `chmod +x pocket.10m.py` in that folder.
4. [Create your consumer key](https://getpocket.com/developer/apps/new) from Pocket's developer console and authorize the app. Copy your consumer key and paste in the Pocket Bar dialog, then press Authorize button in the opened browser tab.

![](https://i.imgur.com/tMuIBuo.png)

![](https://i.imgur.com/xScuD21.png)

![](https://i.imgur.com/z393bL5.png)

6. Start BitBar, or if already running, click the BitBar menu and choose Preferences -> Refresh all.

### tl;dr
```bash
 # install BitBar
 brew cask install bitbar

 # install the Python, Pocket API wrapper and Keyring packages
 brew install python && pip3 install -U pocket-api keyring

 # install the Pocket Bar script to the BitBar plugins folder
 cd "$(defaults read com.matryer.BitBar pluginsDirectory)" && curl -LO https://github.com/inbalboa/pocketbar/releases/latest/download/pocket.10m.py && chmod +x pocket.10m.py
````
Create consumer key, authorize the app & (re)start BitBar.