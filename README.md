# Denier Lab

A 3D stocking simulator web toy — Denier（丝袜的「D 数」）you can play with in the browser, no download needed.

**▶ Play it:** open `index.html` in any browser, or via GitHub Pages once enabled (Settings → Pages → Deploy from branch `main`, folder `/ (root)`) at https://gengannie.github.io/denier-lab/

## What you can adjust

- **Denier 5D–200D** — sheerness computed from the D number in real time (α = 1 − e^(−D/45)), deeper at the silhouette edges, sheerer over the calf
- **Color** — 6 presets plus a custom picker
- **Sheen** — matte to glossy, continuous
- **13 patterns** — plain, fishnet, stripes, rose lace, baroque vine, leopard, hearts, butterfly, stars & moon, houndstooth, argyle, sakura, spiderweb
- **5 lengths** and **8 one-tap preset styles**
- **Load your own model** — drop in any `.vrm` / `.glb` anime model and the tights system applies to it (shoes are stripped automatically)

Drag to turn her, scroll or pinch to zoom. Everything runs locally in one self-contained `index.html` — the model (2.1 MB VRM) is embedded in the file, so there are no external requests.

## Tech

Three.js + WebGL, a skinned tights overlay bound to the model's own body geometry (clipped at the hip line), canvas-generated pattern textures, render-on-demand with shadow baking for smooth turning.

## Credits

- Character: official VRM 1.0 sample avatar © pixiv Inc., used and redistributed under the VRM 1.0 license
- Built with Three.js
