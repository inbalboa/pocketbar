# Pocket Bar

A simple plugin to the [BitBar](https://getbitbar.com/) as basic [Pocket](https://getpocket.com/) client working in your Mac menu bar.

![](https://i.imgur.com/xxtHqaW.png)

Supports main actions: retrieve articles, add or delete (use ⌥) an article.

![](https://i.imgur.com/JAcw7IY.png)

## Instructions

1. Install the latest version of [BitBar](https://github.com/matryer/bitbar/releases/latest). I recommend to use [brew](https://brew.sh/): `brew cask install bitbar`.
2. Open a terminal and run `pip3 install pocket-api`.
3. Copy [pocket.10m.py](pocket.10m.py) to your BitBar plugins folder, and run `chmod +x pocket.10m.py` from your terminal in that folder.
4. [Create your consumer key](https://getpocket.com/developer/apps/new) from Pocket's developer console and authorize the app on your own account (you can use tools such as [fxneumann's OneClickPocket](http://reader.fxneumann.de/plugins/oneclickpocket/auth.php)) to getting the access token. Then, set variables CONSUMER_KEY and ACCESS_TOKEN in the [pocket.10m.py](pocket.10m.py).
6. Start BitBar, or if already running, click the BitBar menu and choose Preferences -> Refresh all.
