# Command Tab

Build a Chrome new-tab workspace with Grok Build: clock, search, shortcut sections, settings, then Edit mode that saves locally.

This is not TidyApply. TidyApply Command is one example for how to refine and publish an extension to the Chrome Web Store.
https://chromewebstore.google.com/detail/tidyapply-%E2%80%94-command/blodgoahghkjdhjkghmknmiabkpjhomn 

Workshop: DataCamp code-along with Ken Rose — *Create a Chrome Extension with Grok Build*.

## Files in this repo

| File | What to do |
|---|---|
| [sketch.png](sketch.png) | Download. In Grok Build, attach it with `@sketch.png` |
| [prompt-1.txt](prompt-1.txt) | Open → copy → paste into Grok Build |
| [prompt-2.txt](prompt-2.txt) | Same, after Version 0 is loaded |

You do not need to clone this repository. Copy the prompts. Download the sketch.

## What you need

- Google Chrome
- Grok Build (`grok --version`)
- SuperGrok or X Premium+ — the grok.com browser chat is not this session
- An empty folder on your machine

## Build it

1. Open a terminal in an empty folder. Run `grok`.
2. Attach the sketch: type `@` and choose `sketch.png`.
3. Paste [prompt-1.txt](prompt-1.txt). Wait until these four files exist:
   - `manifest.json`
   - `newtab.html`
   - `newtab.css`
   - `newtab.js`
4. Load the folder in Chrome (steps below).
5. In the same Grok Build session, paste [prompt-2.txt](prompt-2.txt). Do not start over.
6. Reload the extension card, then open a new tab.

If Prompt 1 has not produced `manifest.json` after several minutes, stop and follow along on the presenter’s screen. You can rerun both prompts after the call.

## Load unpacked

1. Go to `chrome://extensions`
2. Turn on Developer mode
3. Click **Load unpacked**
4. Select the folder that contains `manifest.json`
5. Press Ctrl+T (Cmd+T on Mac)

You should see Command Tab, not Chrome’s default new tab.
Chrome may ask if you agree to the plan of changing the new-tab experience - agree to the change.

After Grok edits files: on `chrome://extensions` click the reload icon on Command Tab, then open a **new** tab. Refreshing an old tab is not the way to test this.

If another new-tab extension is still in control, disable it first.

## Checkpoints

**After Prompt 1:** clock works, a seed tile opens a site, `+` adds a tile, the gear changes the page. There should be no service worker and no TidyApply branding.

**After Prompt 2:** hover a section title for about 300ms — a pencil appears. Click it. The title is editable, `+` shows in that section only, actions sit under the tile name (not on the icon). Clicking a tile does not navigate until you click the check (or press Escape). Open a new tab: your edits are still there.

## What we are not building

Favicons, a focus timer, a to-do list, drag-and-drop across sections, publishing to the Chrome Web Store, or TidyApply.

## After the session

Keep the two prompts. To change the extension, open Grok Build in the same folder and describe one change. Reload the extension card, then open a new tab.
