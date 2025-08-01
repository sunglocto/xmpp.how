## Choosing a client
There are a variety of clients out there. This page will tell you about the ones we recommend. All of these clients support end to end encryption, and use modern features like message history, file uploads and more.

### I use Android
We recommend Conversations or Monocles chat, both of which can be obtained from the Google Play store for a small fee. If you'd like to download these for free, you can get them from F-Droid. Conversations and Monocles chat share the same codebase and inherit many of the same features, but Monocles chat looks a bit nicer and has support for more brand new features.
If you are not interested in F-Droid nor do you want to pay for Conversations or Monocles chat, you can use Snikket, which has fewer features but can get the job done. Please note that if you use Google Play Family Library, you can purchase Conversations once to make it available to your other 5 family members.

### I use Windows.
We recommend Gajim. You can download it [here](https://gajim.org/).

### I use MacOS/iOS.
We recommend Monal IM. You can download it from the App Store. Unfortunately, XMPP on iOS is a bit of a poor experience as of writing. If you use one of the other platforms, you should use XMPP on that. [Why?](#Why are there so few options on iOS?)

### I use GNU/Linux.
We recommend Gajim. It is available in most distros, and there is a Flatpak. You may want to try Dino as well, if you want an ultra simplified experience.

### I use a Chromebook or web browser. / I'm not allowed to install programs on this device.
We recommend ConverseJS. It is extremely simple and plain, so you should use one of the other clients if you're able, but it does have enough features to get by. You can use it  [here](https://chat.conversejs.org/).

### I use a terminal
We recommend Profanity. It's available for Windows, GNU/Linux, MacOS, OpenBSD, FreeBSD, and Android (through Termux). It is as feature rich as Gajim, and is similar to Irssi, so it is very easy to use. (Everything is done through /commands instead of hard to remember key-binds.) Because Profanity uses GNU Readline, you can easily add arbitrary keybinds, and if you use Vi(m) or Emacs, you can setup similar keybinds. You can get it [here](https://profanity-im.github.io/).

## Installed a client?
Great! Now you can [choose a server](Servers.md) to chat on and communicate with others, or even setup your [own server](Host%20your%20own%20server.md) in order to have your own chatroom and be fully independent from others. Be advised that you should update your client frequently in order to take advantage of new XMPP features.

## Clients to avoid
Here are some clients you should not use for one reason or another.

- Pidgin (GNU/Linux, Windows, MacOS): While Pidgin does have protocol support for XMPP, it is extremely simple, and only supports basic text chat (no end to end encryption, no files, no message history).
- Yaxim (Android): Only supports basic text chatting and files (no end to end encryption, no message history). This might be useful if you are using an extremely old or low-spec Android smartphone.
- Psi(+) (GNU/Linux, Windows): Mainly for advanced users. No advanced message history in MUCs, and no message history at all in DMs.
- ChatSecure (iOS): No longer maintained, and has only a few features. You should use Monal instead.

## Why are there so few options on iOS?
*TL;DR version: Notifications are inconsistent on iOS due to how Apple has designed their operating system.*

### Full Explanation:
XMPP works by maintaining a background connection to the server you're connected to in the background.

This works fine on Android, Windows, GNU/Linux, and MacOS, but on iOS, Apple states that apps are not allowed to be programmed to run in the background if they wish to be on the App Store. There is a workaround many servers will enable, but it doesn't always work and Apple may break these implementations at any one time. This causes notifications to be inconsistent and a worsened user experience.