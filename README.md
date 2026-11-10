# שלח לך: תעלומת המשלחת האבודה

A static website: no server, database, accounts or API keys.

## Publish on GitHub Pages
1. Create a repository (for example `shlach-lecha`) and upload **the contents of this folder**: `index.html`, `README.md` and the whole `assets/` folder, keeping the folder structure.
2. In the repository: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)` → **Save**.
3. After a minute or two, the game is at `https://<your-username>.github.io/<repository-name>/`.

## Files
| File | Purpose |
| --- | --- |
| `index.html` | The whole game: code, styles, fonts and all text content |
| `assets/op_bg_camp_dawn.webp` | Opening: the camp at dawn (also the title screen and the memory scene) |
| `assets/op_bg_tent_interior.webp` | Joshua's command tent (opening and final station) |
| `assets/op_bg_camp_edge.webp` | Edge of the camp (opening) and the lookout (Station 2, cropped) |
| `assets/s1_bg_riverbank.webp` | Jordan riverbank (Station 1) and Jericho at night (Station 3, cropped) |
| `assets/chr_joshua_portrait.webp`, `assets/chr_stranger_portrait.webp` | Dialogue portraits, cropped from the approved references |

## Replacing or adding artwork
Replace any image with a new file of the **same name** (2560×1440 WebP for backgrounds) and the game uses it automatically. If an image fails to load, the scene shows a dark fallback with a small notice, and play continues.
To give a station its own background, add the file to `assets/` and point that station's `scene()` at it in `index.html`. The station definitions are in the `STATION_DEFS` section; tap areas are given in pixels of a 2560×1440 image.

## Teacher mode
Click the "שלח לך" logo three times and enter the code `מורה`. It uses a separate save and never touches a student's progress.

## Saving
Progress saves automatically in the browser. To move to another device, a student uses 💾 → "שליחת ההתקדמות למייל" and, on the other device, "המשך משחק משמירה".
