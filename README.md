# xfce4 Mullvad VPN status plugin

This repository offers a script, which reads your VPN status from [Mullvad](https://mullvad.net/en/) API
and presents them on Xfce panel using [xfce4-genmon-plugin](https://docs.xfce.org/panel-plugins/xfce4-genmon-plugin).

## Screenshots

When you are connected to Mullvad VPN:

![Connected](media/connected.png)

And when you are disconnected:

![Disconnected](media/disconnected.png)

## Installation

Copy the script to your PATH, for example to `~/.local/bin`:

```sh
mkdir -p ~/.local/bin
cp mullvad-status ~/.local/bin/
```

## Adding to Panel

Add new `xfce4-genmon-plugin` to your panel and configure it to run the following command:

```sh
.local/bin/mullvad-status
```
