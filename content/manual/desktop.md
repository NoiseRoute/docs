---
title: Noise Route Desktop
geekdocNav: true
geekdocAlign: start
geekdocAnchor: true
---

{{< hint type=important title="Alpha" >}}
Noise Route is currently in alpha version, things may be changed in the future
{{< /hint >}}


# Install
You may need an account and verified your email before downloading `Noise Route Desktop`, you can [register](https://noiseroute.com/register) or [login](https://noiseroute.com/login)

## Supported OS

| OS Name | Type                                          | Feature         |
| ------- | --------------------------------------------- | --------------- |
| Windows | `x64`                                         | Send/Play audio |
| Linux   | `Ubuntu 22.04` `Ubuntu 20.04`  `Ubuntu 18.04` | Send/Play audio |

> ### MacOS
> Due to security reasons, MacOS does not expose API for audio capturing, so MacOS support may come later.

## Start Noise Route
After Noise Route is succesfully installed on your system, you can start the program.
> On ubuntu, you can start noise route by running `noise-route` from terminal, if you want to run it in background, you can run `noise-route &`

## Alpha notice
By the first times you start the program, you will see a pop up like so:

![alpha notice](/images/alpha-notice.png)

This pop up will keep showing up until you click `I understand` twice, and then another option will show up in the next time:

![another option](/images/pop-up-another-option.png)

After you clicked `OK, don't show again`, it will not show again(unless you deleted the config file).

## Add device
Since desktop versions has two modes, how to add device in each mode is different.
### Add device in playing mode.
By clicking the "`+`" icon on top right, a pop up will show, which you can type in the ip address of audio sending pc, and you can find the ip address of that device by reading [next section](#add-device-in-sending-mode)

### Add device in sending mode.
You can click the "`+`" icon on top right, and a add device helping screen will show up, which contains informations you may need for adding device to send audio to.

![add device info](/images/send-add-device.png)



## Switching modes
By default, `Noise Route Desktop` is in `send audio` mode, as you can see at the top bar, but it can also receives audio if you want(then you need another desktop to send audio from), and you can do this by following these steps:

1. click the gear icon on top right and into settings.

![settings send audio](/images/settings-send.png)

2. switch toggle saying `Send audio`, you should see the text chaged to `Play audio` and the toggle button changed from yellow to blue.

![settings play audio](/images/settings-play.png)

And you are in play audio mode and start receiving audio.
