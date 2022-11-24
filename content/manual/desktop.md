---
title: Noise Route Desktop
geekdocNav: true
geekdocAlign: start
geekdocAnchor: true
---

{{< hint type=important title="Beta" >}}
Noise Route is currently in beta version.
{{< /hint >}}

# Install
You can download `Noise Route Desktop` in [https://noiseroute.com/download](https://noiseroute.com/download)

## Supported OS

| OS Name | Type                                          | Feature supported |
| ------- | --------------------------------------------- | ----------------- |
| Windows | `x64`                                         | Send & Play audio |
| Linux   | `Ubuntu 22.04` `Ubuntu 20.04`  `Ubuntu 18.04` | Send & Play audio |

> ### MacOS
> Due to security reasons, MacOS does not expose API for audio capturing, so MacOS support may come later.

## Before connecting
Before connecting to device, make sure the device sending audio and the device receiving audio are in the same local network(in the same wifi).

## Start Noise Route
After Noise Route is succesfully installed on your system, you can start the program.
> On ubuntu, you can start noise route by running `noise-route` from terminal, if you want to run it in background, you can run `noise-route &`

## Add device
Since desktop versions has two modes, how to add device in each mode is different.
### Add device in playing mode.
By clicking the "`+`" icon on top right, a pop up will show, which you can type in the ip address of audio sending pc, and you can learn how to find ip addres by reading [next section](#add-device-in-sending-mode)

### Add device in sending mode.
You can click the "`+`" icon on top right, and a add device helping screen will show up, which contains informations you may need for adding device to send audio to.

![add device info](/images/send-add-device.png)

As you see above, the pop up contains:
* ip address of your pc.
* QRCode ([how to add device using QRCode](../mobile#scan-qrcode))

If you have an account with active subscription logged in, TLS encryption will be enabled, and TLS fingerprint will show:
![add device show tls fingerprint](/images/send-add-device-with-fingerprint.png)

## Switching modes
By default, `Noise Route Desktop` is in `send audio` mode, as you can see at the top bar, but it can also receives audio if you want(then you need another desktop to send audio from), and you can do this by following these steps:

1. click the gear icon on top right and into settings.

![settings send audio](/images/settings-send.png)

2. switch toggle saying `Send audio`, you should see the text chaged to `Play audio` and the toggle button changed from yellow to blue.

![settings play audio](/images/settings-play.png)

And you are in play audio mode and start receiving audio.

# Advance features

## Channel selecting
If you have account logged in, by clicking `Channel:` you will see the channel selecting option once the device item expanded:
![channel select](/images/channel_select.png)

And by selecting different option, you can set device to playing specific channel only, and you can see the icons updated on both end:
![channel select on sending](/images/channel-select-tx.png)


on playing device:

<img src="/images/channel-select-rx.png" width="400px">

# Premium features
Premium feature require an account with active subscription or trial logged in.

Options for premium features are only configurable in send audio mode.

## TLS encrypted communication
After you logged in, TLS encrypted communication will be enabled automatically, and it can't be turned off until your subscription was not longer valid or logged out.

![logged in with valid subscription](/images/logged-in.png)

### regenerate tls certificate
By clicking on `TLS encryption`,you can see the current tls certificate fingerprint.
![show tls fingerprint](/images/show-tls-fingerprint.png)

By clicking the `Regenerate` button, your certificate will be regenerated, and connections with current connected devices will be reset.

## AES audio encryption
AES audio encryption is not enabled by default after you logged in, since this will increase compute time and resources, you can turn in on by clicking the toggle.

![audio enc turned on](/images/aes-audio-enc-option.png)

By clicking on `Audio encryption`, you can see the audio encryption information
![audio enc info](/images/audio-end-info.png)


By turning on/off AES audio encryption, connections with current connected devices will be reset, each time audio enc was turned on or application starts, the audio enc infomations will be regenerated.
