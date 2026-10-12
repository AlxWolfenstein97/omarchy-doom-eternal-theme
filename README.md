# Doom Eternal — Omarchy theme

Rip and Tear, until it is DONE! Mick Gordon's Metal Choir has yet to reach
our hypr systems, cliamp some more. What if your desktop matched Eternal’s
**blood red → hellfire orange** instead of 2016’s praetor green dual-accent?
Same Hyprland border trick as Asphalt, HEV, Galuga, CS, Cyber Shadow, Doom 2016, Caged, KI, Rising, Stanley, SF6, T2D & USFIV —
warmer void, louder crimson. Pure `#FE0000` stays on
`accent` (Limine / borders); the ANSI row is pastelized so OmaVT / getty
actually pops — different slots, not a plugin bug.

Slayer theme for [Omarchy](https://omarchy.org/). Inspired by the look of
*DOOM Eternal* — **not affiliated with id Software or Bethesda Softworks** (see
[Credits](#credits--legal-ish) below).

No Omarchy “DOOM Eternal” pack turned up. The closest hit was
[AX200M/omarchy-doom-theme](https://github.com/AX200M/omarchy-doom-theme) —
that’s **MF DOOM** (the rapper), not the game. Palette cues borrowed from
Jacob Westall’s COSMIC
[Rip And Tear Dark](https://cosmic-themes.org/?search=Rip+And+Tear)
(`accent` / `bg_color` blood tint). Windows ExpoThemes wallpaper packs exist,
but they’re logo-heavy and don’t port cleanly. Built from Steam store /
library art and Wallhaven key art the same way as
[Asphalt Legends](https://github.com/AlxWolfenstein97/omarchy-asphalt-legends-theme),
[HEV Suit](https://github.com/AlxWolfenstein97/omarchy-hev-suit-theme),
[Operation Galuga](https://github.com/AlxWolfenstein97/omarchy-operation-galuga-theme),
[Counter-Strike](https://github.com/AlxWolfenstein97/omarchy-counter-strike-theme),
[Cyber Shadow](https://github.com/AlxWolfenstein97/omarchy-cyber-shadow-theme),
[Doom 2016](https://github.com/AlxWolfenstein97/omarchy-doom-2016-theme),
[Half-Life Caged](https://github.com/AlxWolfenstein97/omarchy-half-life-caged-theme),
[Killer Instinct](https://github.com/AlxWolfenstein97/omarchy-killer-instinct-theme),
[Metal Gear Rising](https://github.com/AlxWolfenstein97/omarchy-metal-gear-rising-theme),
[Stanley Parable](https://github.com/AlxWolfenstein97/omarchy-stanley-parable-theme),
[Street Fighter 6](https://github.com/AlxWolfenstein97/omarchy-street-fighter-6-theme),
[Terminator 2D: NO FATE](https://github.com/AlxWolfenstein97/omarchy-terminator-2d-no-fate-theme),
and
[Ultra Street Fighter IV](https://github.com/AlxWolfenstein97/omarchy-ultra-street-fighter-iv-theme).

<p align="center">
  <img src="logo.png" alt="DOOM Eternal wordmark used for unlock / README" width="520" />
</p>

![Desktop preview](preview.png)

![Unlock / Plymouth preview](preview-unlock.png)

## Install

```bash
omarchy theme install https://github.com/AlxWolfenstein97/omarchy-doom-eternal-theme.git
# optional — About + screensaver ASCII for this theme (skippable; see Branding)
cp ~/.config/omarchy/themes/doom-eternal/about.txt ~/.config/omarchy/branding/about.txt
cp ~/.config/omarchy/themes/doom-eternal/screensaver.txt ~/.config/omarchy/branding/screensaver.txt
```

That clones **and** applies the theme (`omarchy-theme-set` runs inside
`theme install`). Do **not** follow with another `omarchy theme set` — a second
set skips the first wallpaper and just wastes a switch.

Or clone into place (then you *do* need an explicit set):

```bash
git clone https://github.com/AlxWolfenstein97/omarchy-doom-eternal-theme.git ~/.config/omarchy/themes/doom-eternal
omarchy theme set "Doom Eternal"
# optional branding — same as above
cp ~/.config/omarchy/themes/doom-eternal/about.txt ~/.config/omarchy/branding/about.txt
cp ~/.config/omarchy/themes/doom-eternal/screensaver.txt ~/.config/omarchy/branding/screensaver.txt
```

Already installed and just switching back later:

```bash
omarchy theme set "Doom Eternal"
# optional — re-apply this theme’s About / screensaver marks
cp ~/.config/omarchy/themes/doom-eternal/about.txt ~/.config/omarchy/branding/about.txt
cp ~/.config/omarchy/themes/doom-eternal/screensaver.txt ~/.config/omarchy/branding/screensaver.txt
```

Cycle wallpapers with `omarchy theme bg next`.

## What’s in the pack

| Asset | Role |
|-------|------|
| `colors.toml` | Palette (the real theme) |
| `backgrounds/` | HUD-less / logo-free wallpapers |
| `unlock.png` / `preview-unlock.png` | Plymouth unlock + picker mockup |
| `preview.png` | Theme switcher preview |
| `icon.txt` / `logo.txt` (+ `about.txt` / `screensaver.txt`) | About & screensaver **ASCII** branding |
| `icon.png` / `logo.png` | Same marks as images (README + optional “Set From Image”) |

### Branding (About / screensaver)

**Optional.** Omarchy’s About screen and screensaver read from
`~/.config/omarchy/branding/`. Shipping per-theme `.txt` marks isn’t original —
other Omarchy 3.x themes did it — but it’s the fast path if you want *this*
pack’s wordmark on idle and on About without hunting files.

**Prefer the `.txt` files** and the `cp` lines in [Install](#install). That’s
what you’re meant to see. Editing the text also works (Style → About /
Screensaver → Edit Text).

**Skip the `cp` if you already have custom logos / screensaver art you care
about** — or back those up first. The branding slot is really meant for *your*
marks (put personal art somewhere easy to reach). The Style file picker works,
but drilling into `~/.config/omarchy/themes/...` is slow busywork for something
optional. Don’t feel obliged to bring mine.

The `.png` versions are here for the README and for a quick Style → **Set From
Image** try. In my experience Omarchy’s image→ASCII path is a bit thinicky on
color and boxing, so don’t expect magic from the PNGs — the hand text is the
good path.

Screensaver / logo ASCII has **no empty lines** (dense pack: 2016-style
sawtooth **DOOM** wordmark + the Eternal red **ETERNAL** plaque underneath).
About / icon is a Mark of the Slayer silhouette.

### Unlock

Style → Unlock → pick this theme (`unlock.png` / `preview-unlock.png`).

## Extend further with plugins

This repo is **palette + assets** on purpose. Omarchy already colour-coordinates
the shell, terminals, and editor from `colors.toml`. The plugins below push that
idea as far as it can reasonably go — optional extenders, not required theme
baggage. Themes keep working without them; authors can stick to the snappier
stock pipeline if they prefer.

They do **not** depend on each other. Pick what you want; run the whole
inch-a-lada if you want the desktop to feel like yours.

### The big sweep

| Plugin | What it themes |
|--------|----------------|
| **[Chroma](https://github.com/AlxWolfenstein97/chroma)** | GTK3 / GTK4 / libadwaita + Qt |
| **[OmaOBS](https://github.com/AlxWolfenstein97/omaobs)** | OBS Studio (real Yami `Omarchy.ovt`) |
| **[OmaCursor](https://github.com/AlxWolfenstein97/omacursor)** | Pointer / Adwaita XCursor recolor (+ optional SDDM) |
| **[OmaHud](https://github.com/AlxWolfenstein97/omahud)** | MangoHud colours only — live in-game retint |
| **[OmaBoot](https://github.com/AlxWolfenstein97/omaboot)** | Limine boot menu colours |
| **[OmaVT](https://github.com/AlxWolfenstein97/omavt)** | Virtual console / TTY palette |
| **[OmaTTY](https://github.com/AlxWolfenstein97/omatty)** | Console font (Terminus-first, accessibility) |

**Boom-in — one paste.** `--enable --yes` skips the per-plugin clone/enable
prompts; arm-all then arms deps + Style/theme-set + root/SDDM/DRM (no Y/n).
Omit any `plugin add` line you do not want; arm-all only touches what is
installed. Sudo may ask once — that is the boom, not a menu.

```bash
omarchy plugin add https://github.com/AlxWolfenstein97/chroma.git --enable --yes
omarchy plugin add https://github.com/AlxWolfenstein97/omaobs.git --enable --yes
omarchy plugin add https://github.com/AlxWolfenstein97/omacursor.git --enable --yes
omarchy plugin add https://github.com/AlxWolfenstein97/omahud.git --enable --yes
omarchy plugin add https://github.com/AlxWolfenstein97/omaboot.git --enable --yes
omarchy plugin add https://github.com/AlxWolfenstein97/omavt.git --enable --yes
omarchy plugin add https://github.com/AlxWolfenstein97/omatty.git --enable --yes
~/.config/omarchy/plugins/io.github.alxwolfenstein97.chroma/tools/arm-all-family.sh
```

**Boom-out — one paste.** Teardown + ledger pkg drop + plugin remove.
Ledger drops only what we recorded pulling; may fail and stay if something else
still needs the package (e.g. Goverlay after Pillow) — fine. Loud boom-in after
this is enough — no tombstone purge needed (optional OCD flag lives on the
plugin READMEs).

```bash
~/.config/omarchy/plugins/io.github.alxwolfenstein97.chroma/tools/wipe-all-family.sh
```

**Piece-meal** (not boom): one plugin’s Workshop paste — `plugin add` + interactive
`install.sh` (asks [Y/n]) — lives on that plugin’s GitHub README. Single-plugin
full wipe: `…/<plugin>/uninstall.sh --yes`.

### Already solved elsewhere (gladly)

- **[Omacord](https://github.com/ASwenia/omacord)** — Vesktop / Vencord Discord
  follows Omarchy themes live:  
  `omarchy plugin add https://github.com/ASwenia/omacord --enable`

### Agent / desktop bridge

- **[OMCP](https://github.com/btsouth/omarchy-omcp)** — MCP desktop bridge:  
  `omarchy plugin add https://github.com/btsouth/omarchy-omcp --enable`

Browse more on the [Omarchy Plugins](https://plugins.omarchy.org/) site.

## Taste

Colours and contrast are tuned for what I like to look at. If they feel loud or
wrong for you, fork and retune `colors.toml` without guilt.

## Credits / legal-ish

- Visual inspiration and reference art from **id Software** / **Bethesda
  Softworks**’ *DOOM Eternal* branding and marketing (Steam library hero / logo,
  official key art, HUD-less Steam store screenshots). **Not affiliated with,
  endorsed by, or sponsored by id Software or Bethesda Softworks.** Just public
  pixels arranged into an Omarchy theme — no money, no official product.
- Colour cues from Jacob Westall’s COSMIC **Rip And Tear Dark** (pure-red
  accent + blood-tinted background) — remapped into Omarchy `colors.toml`, not
  a port of the `.ron`.
- Wallhaven IDs used for key art: `73k5ko` (crucible triumph), `mdwr99` (Khan
  Maykr), `5wr1m8` (Marauder axe battle), `3zlo63` (Ancient Gods), `zmovwg`
  (Mars core).
- Steam store shots used for the praetor helm, Hell on Earth city, Mancubus
  riposte, and plasma corridor were checked for HUD and title overlays before
  shipping — logo-bearing capsules / Wallhaven logo comps were dropped on
  purpose.
- If id or Bethesda hates this existing, they can say so and I’ll deal with the
  repo accordingly.

## License

Do whatever you want with this theme pack unless id Software, Bethesda Softworks
(or the law) says otherwise. Fork it, recolor it, ship it in a rice. No warranty
— it’s wallpaper and hex codes.
