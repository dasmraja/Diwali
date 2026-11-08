# 🪔 Light a Diya — an interactive Diwali greeting

A single-file, no-install Diwali greeting that runs in any browser (phone or desktop) and is designed to be sent over WhatsApp.

**How it plays**

1. The receiver opens the link and sees *"Priya sent you a Diwali wish — Tap the diya to light it"*.
2. Their tap throws a spark to the middle diya, and the flame passes from diya to diya, each one ringing a soft bell note.
3. A rangoli blooms layer by layer, drawn by a point of light, with sky lanterns rising behind it.
4. *शुभ दीपावली / Happy Diwali, Rohan* fades in with the sender's wish, and fireworks start. One shell bursts in the shape of a diya.
5. Every tap after that launches a firework where they tapped. At the end they can **Send to someone**, **Personalise** their own version, or **Replay**.

Everything is drawn on a canvas and the sound is made in the browser, so there are no images, audio files or libraries to load.

## Personalise via the link

| Parameter | Example | Shown as |
|-----------|---------|----------|
| `from`    | `from=Priya%20%26%20family` | "Priya & family sent you a Diwali wish" / "— with love, …" |
| `to`      | `to=Rohan` | "Happy Diwali, Rohan" |
| `msg`     | `msg=Wishing%20you%20light…` | replaces the default wish (max 160 chars) |

Example: `https://dasmraja.github.io/diwali/?from=Priya&to=Rohan`

The **Personalise** button builds this link for you and opens WhatsApp with a ready-made message (on phones it opens the app; on desktop it opens WhatsApp Web).

## Publish it (GitHub Pages)

WhatsApp needs a public `https://` link, so the page has to be hosted:

1. On GitHub, go to **Settings → Pages**.
2. Under **Source**, choose **Deploy from a branch**, then pick the branch and the `/ (root)` folder.
3. The greeting will be live at `https://dasmraja.github.io/diwali/`.

`og-image.png` is the preview card WhatsApp shows with the link. Its URL in `index.html` (`og:image`) assumes the GitHub Pages address above, so change it if you host somewhere else.

To try it locally, open `index.html` in a browser.
