# NastyTavern × Donsac

## What

Single SillyTavern extension = **NastyTavern UX** + **Donsac** black/muted-blue style baked into `style.css`. No separate theme JSON required.

- Upstream features: [AnNastyLoneGirl/NastyTavern-UI](https://github.com/AnNastyLoneGirl/NastyTavern-UI) `0.1.14`
- Style: Donsac theme (black / `#d6d6d6` text, muted steel-blue accent `#7a9bb8`, square chrome, Arsenal/Saira/Voltaire)
- Fork version: `0.1.14-donsac.9`
- Repo: **private** — Install from URL may need GitHub auth (see below)

## Install

1. **Disable or remove stock NastyTavern UI** (`AnNastyLoneGirl/NastyTavern-UI`) first. Both inject the same shell (`body.mt-enabled`) and will conflict.
2. SillyTavern **1.18.0+**.
3. **Extensions → Install extension** and paste:

   `https://github.com/literallywhatisthis/nastytavern-donsac`

4. Because this repo is **private**, Install-from-URL often fails without GitHub authentication. Options:
   - Configure git credentials on the SillyTavern host (HTTPS **PAT** with `repo` scope, or SSH key that can read this private repo), then retry Install extension.
   - **Manual clone** into the third-party extensions folder, e.g.  
     `git clone https://<TOKEN>@github.com/literallywhatisthis/nastytavern-donsac.git`  
     into `data/<user>/extensions/` or `public/scripts/extensions/third-party/`.
   - Download a zip from GitHub while signed in, unpack so `manifest.json` is at the folder root, copy into the extensions directory.
5. Reload SillyTavern and enable **NastyTavern × Donsac**.

### Already installed?

`git pull` (or re-copy the latest package), then **reload the extension / hard-refresh SillyTavern** so `style.css` updates. `auto_update` is off.

## Chat Appearance

In **NastyDonsac / NastyTavern Settings → Chat Appearance**, keep values on **Inherit / Theme** where possible so baked message chrome wins. Custom Chat Appearance overrides can undo the Donsac layout.

`auto_update` is **false**. Do not point SillyTavern’s update remote at stock NastyTavern — that would wipe the Donsac overlay.

## Credits

- Feature code / UX: [AnNastyLoneGirl/NastyTavern-UI](https://github.com/AnNastyLoneGirl/NastyTavern-UI)
- Visual language: Donsac theme
