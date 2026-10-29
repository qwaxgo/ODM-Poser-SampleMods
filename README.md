# SymbolicPoseEditor-SampleMods

Sample mods for the Symbolic Pose Editor (ComfyUI-SymbolicPoseEditor). Private.

| file | adds |
|------|------|
| `hello_mod.js` | a category with a star wand, a halo and devil horns; an eight-sided pillar; a dashed-ring aura and an aura part for the feet; the hand shape "three fingers"; a waving pose; English words; a panel that draws a plumb line from the head (`draw` hook, kept in `api.data()`) |

## Install

Clone this repository into the editor's `mods/` folder; every `*.js` at its top level loads as a mod.

```
cd ComfyUI/custom_nodes/ComfyUI-SymbolicPoseEditor/mods
git clone git@github.com:qwaxgo/SymbolicPoseEditor-SampleMods.git
```

- Inside ComfyUI: reload the editor (after updating the node itself, restart ComfyUI once).
- Opened from disk: run `python tools/make_mods_list.py` in the editor's folder, then reload.
- To turn one mod off, rename it to start with `_` (for example `_hello_mod.js`).

The editor's `mods/` folder is git-ignored, so this repository lives there on its own.

How to write a mod: `docs/MODDING.md` / `docs/MODDING-JA.md` in the editor's repository.

## 日本語

記号ポーズエディタのサンプル MOD（非公開）。エディタの `mods/` フォルダにこのリポジトリを clone すると、
直下の `*.js` が MOD として読み込まれます。ComfyUI の中ならエディタを開き直すだけ、ComfyUI なしで開くときは
エディタのフォルダで `python tools/make_mods_list.py` を実行してから開き直します。
