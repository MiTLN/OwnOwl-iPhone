<p align="center"><img src="icon.png" width="120" alt="OwnOwl"></p>

# OwnOwl - a private AI chat that runs on your iPhone

OwnOwl runs a large language model **entirely on your iPhone**. No internet is
used for chatting, and your conversations never leave your device. It speaks
several languages, remembers facts about you only when you confirm them, and
chats in a familiar messenger-style interface.

> **This is a time-limited TEST build for evaluation only.** It stops working
> after a built-in expiry date. Please read [LICENSE.md](LICENSE.md) before you
> install it. For evaluation and testing only - no commercial use, no
> redistribution.

---

## What's new in v0.2

- **Much faster first reply.** The app warms up when it loads and remembers each
  conversation, so reopening a chat and asking again answers almost instantly
  instead of re-reading the whole history.
- **Answer length & "Continue".** Longer answers by default, and a **Continue**
  button to extend a reply that reached its length limit.
- **Clearer status while answering:** *thinking…* then *typing…*, with a spinner
  while the model is thinking.
- **Lighter on memory.** When you leave the app it frees the model from memory
  and reloads it when you come back.
- **Memory about you.** It can remember facts about you - only the ones you
  confirm - and use them in later answers.
- **Stability fixes:** no more crashes when the app goes to the background or on
  long answers; smoother scrolling when you send a message.

---

## Requirements

- **An iPhone with 6 GB of RAM or more.** This is required. Examples that work:
  iPhone 12 Pro, **13 Pro**, 14 / 14 Plus / 14 Pro / Pro Max, 15 and newer,
  and iPads with an M1 chip or newer.
  Phones with 4 GB of RAM (e.g. the regular iPhone 11, 12, 13) are **not**
  supported and the larger models will not fit.
- **iOS 17 or newer.**
- **Free storage** for the model you choose: about 6 GB (GigaChat), 9 GB (Ling),
  or 14 GB (Gemma). Download over Wi-Fi.
- A **Mac or Windows PC** is needed once, to install the app (see below).

Speed depends on the phone. On an iPhone 13 Pro: GigaChat ~7 words/second,
Ling ~12, Gemma ~3. Newer phones with 8 GB of RAM are faster.

---

## How to install

Apple does not allow installing an app straight from GitHub. You install the
`.ipa` file from the [Releases](../../releases) page with a free tool that signs
it with **your own Apple ID**. The app is not jailbroken and needs no special
account. Pick one of the two methods.

### Option A - AltStore (recommended; re-signs itself automatically)

1. On your computer, install **AltServer** from https://altstore.io and run it.
2. Connect your iPhone by cable, or keep it on the same Wi-Fi as the computer.
3. In AltServer, choose **Install AltStore** onto your iPhone and sign in with
   your Apple ID (a free account is fine).
4. On the iPhone, open **Settings → General → VPN & Device Management**, tap your
   Apple ID under *Developer App*, and tap **Trust**.
5. Download `OwnOwl.ipa` from the [Releases](../../releases) page onto the iPhone
   (or the computer).
6. Open the **AltStore** app on the iPhone → **My Apps** → **+** → pick
   `OwnOwl.ipa`.
7. **Turn on Developer Mode** when iOS asks: **Settings → Privacy & Security →
   Developer Mode → On**, then restart.

AltStore can refresh the app automatically while your computer is on the same
network, so you rarely have to repeat this.

### Option B - Sideloadly (one-off install)

1. Install **Sideloadly** from https://sideloadly.io on your Mac or PC and open it.
2. Connect the iPhone by cable.
3. Drag `OwnOwl.ipa` into Sideloadly, enter your Apple ID, and click **Start**.
4. On the iPhone: **Settings → General → VPN & Device Management** → tap your
   Apple ID → **Trust**.
5. **Settings → Privacy & Security → Developer Mode → On**, then restart.

### The 7-day note (free Apple ID)

Apps signed with a **free** Apple ID stop opening after **7 days** - this is an
Apple limit, not OwnOwl. Just reinstall with the same steps; AltStore can do it
for you automatically. Your chats and downloaded models stay on the phone.

---

## First launch

1. Open OwnOwl. It asks you to **pick a model** and downloads it from Hugging
   Face. The download runs in the background (keep the app installed; use Wi-Fi
   for the big models).
2. When it is ready, start chatting. Everything runs on the phone, offline.
3. You can add or remove models any time in **Settings → Download or delete
   models**.

---

## Privacy

Your chats are processed and stored **only on your iPhone**. OwnOwl does not send
your messages anywhere. The only network use is downloading the model files you
choose, from Hugging Face.

---

## Feedback

Found a bug or have an idea? Please open an
[Issue](../../issues) - measurements from your device (model, phone, speed) are
especially welcome.

---

## License & ownership

OwnOwl's app and its on-device inference engine are proprietary and **not** open
source. This repository distributes a **test build for evaluation only**; see
[LICENSE.md](LICENSE.md). Third-party libraries and the AI models have their own
licenses - see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

Each test build carries a cryptographic authorship signature and a built-in
expiry, which are part of the App's protection and identify its origin.

© 2026 Mihhail (github.com/MiTLN).
