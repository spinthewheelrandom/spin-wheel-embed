# Spin Wheel Embed 🎡

Add a free, interactive **spin the wheel** to any website, blog, LMS or Notion page with one line of HTML.
Wheels are served by [SpinTheWheelRandom.com](https://spinthewheelrandom.com): a random name picker, yes/no wheel, number wheel, team generator and 20+ themed wheels.

- Free. No sign-up, no API key.
- Works on desktop and mobile.
- Provably fair: every result is picked with Web Crypto and comes with a SHA-256 proof.
- Your entries stay in the visitor's browser.

**[Live demo →](https://spinthewheelrandom.github.io/spin-wheel-embed/)**

---

## Quick start

Paste this where you want the wheel to appear:

```html
<iframe src="https://spinthewheelrandom.com/"
        width="100%" height="680"
        style="border:0;border-radius:16px;overflow:hidden;"
        allow="fullscreen" loading="lazy"
        title="Spin the wheel – random name picker"></iframe>
<p style="font-size:13px">Wheel by <a href="https://spinthewheelrandom.com/">SpinTheWheelRandom.com</a></p>
```

## Ready-made wheels

Swap the `src` for any of these:

| Wheel | `src` |
| --- | --- |
| Random name picker | `https://spinthewheelrandom.com/` |
| Yes or No wheel | `https://spinthewheelrandom.com/yes-or-no-wheel/` |
| Random number wheel | `https://spinthewheelrandom.com/random-number-wheel/` |
| Random letter wheel | `https://spinthewheelrandom.com/random-letter-wheel/` |
| What to eat wheel | `https://spinthewheelrandom.com/what-to-eat-wheel/` |
| Truth or dare wheel | `https://spinthewheelrandom.com/truth-or-dare-party-wheel/` |
| Random team generator | `https://spinthewheelrandom.com/random-team-generator/` |

All wheels: [spinthewheelrandom.com](https://spinthewheelrandom.com/)

## Embed your own wheel (your names, your colours)

1. Open [spinthewheelrandom.com](https://spinthewheelrandom.com/) and type your entries.
2. Click **Share / Embed**.
3. Copy the **Website Embed Code**. It looks like this:

```html
<iframe src="https://spinthewheelrandom.com/?s=YOUR_WHEEL_ID&mode=readonly"
        width="100%" height="680"
        style="border:0;border-radius:16px;overflow:hidden;"
        allow="fullscreen" loading="lazy"></iframe>
```

`mode=readonly` means visitors can spin your wheel but cannot change the list. They can still make their own copy.

## Responsive embed (recommended)

The wheel is easier to use on phones with a taller frame:

```html
<div style="max-width:900px;margin:auto">
  <iframe src="https://spinthewheelrandom.com/yes-or-no-wheel/"
          style="width:100%;height:680px;border:0;border-radius:16px;"
          allow="fullscreen" loading="lazy" title="Yes or No wheel"></iframe>
</div>
<style>@media (max-width:600px){iframe[title="Yes or No wheel"]{height:820px!important}}</style>
```

See [`examples/`](examples/) for complete pages.

## Platform guides

| Platform | How |
| --- | --- |
| WordPress | Add a **Custom HTML** block and paste the code. |
| Blogger | Layout → **Add a Gadget** → HTML/JavaScript, or switch the post editor to HTML view. |
| Google Sites | Insert → **Embed** → Embed code. |
| Notion | Type `/embed` and paste the wheel URL (not the iframe code). |
| Wix / Squarespace | Add an **Embed / Code** block and paste the code. |
| Moodle / Canvas | Switch the editor to HTML and paste the code. |

## Options

| Attribute | Default | Notes |
| --- | --- | --- |
| `height` | `680` | Use 760–820 on narrow mobile layouts. |
| `allow="fullscreen"` | on | Lets viewers use the **Full Screen** button (great for classrooms and projectors). |
| `loading="lazy"` | on | The wheel loads only when scrolled into view, so it does not slow your page. |
| `mode=readonly` | — | Only for your own saved wheels (see above). |

## FAQ

**Is it free?** Yes, including for schools, streams and commercial sites.

**Is the result really random?** Each spin uses the browser's Web Crypto random generator and shows a SHA-256 seed and hash you can verify.

**Do you store my entries?** The standard wheels keep entries in the visitor's browser. A wheel you share with **Share / Embed** is saved so its link can load it. See the [privacy policy](https://spinthewheelrandom.com/privacy-policy/).

**Can I use it in OBS / live streams?** Yes. Use **Share / Embed → OBS Browser Source** on the site.

## License

The example code in this repository is MIT licensed. The wheel itself is a free hosted service of [SpinTheWheelRandom.com](https://spinthewheelrandom.com/).
