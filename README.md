# ODM-Poser-SampleMods

Sample mods for **ODM Poser** (Omni-Directional Mannequin Poser; Japanese name 立体人形装置), the
stick-and-circle pose editor ([ODM-Poser](https://github.com/qwaxgo/ODM-Poser)). They show how to
write a mod with its MOD API.

| file | adds |
|------|------|
| `hello_mod.js` | a category with a star wand, a halo and devil horns; an eight-sided pillar; a dashed-ring aura and an aura part for the feet; the hand shape "three fingers"; a waving pose; English words; a panel that draws a plumb line from the head (`draw` hook, kept in `api.data()`) |

## Use them

Pick the way that fits where the editor runs:

- **In the editor's MOD panel** (any browser, a site such as GitHub Pages, the installed app, a
  phone): **Add by URL** with
  `https://raw.githubusercontent.com/qwaxgo/ODM-Poser-SampleMods/main/hello_mod.js`
  (it loads the latest version every time), or download `hello_mod.js` and **Install from a file**.
- **The editor opened from its folder**: clone this repository into the editor's `mods/` folder,
  then run `python tools/make_mods_list.py` in the editor's folder and reload.
  ```
  cd ODM-Poser/mods
  git clone https://github.com/qwaxgo/ODM-Poser-SampleMods
  ```
- **In ComfyUI** (with [ODM-Poser-ComfyUIBridge](https://github.com/qwaxgo/ODM-Poser-ComfyUIBridge)):
  clone this repository into the bridge's `mods/` folder and reopen the editor.
  ```
  cd ComfyUI/custom_nodes/ODM-Poser-ComfyUIBridge/mods
  git clone https://github.com/qwaxgo/ODM-Poser-SampleMods
  ```

To turn one mod off, rename it to start with `_` (for example `_hello_mod.js`), or switch it off in
the MOD panel. How to write a mod: `docs/MODDING.md` in the editor's repository.

## 日本語

立体人形装置（ODM Poser）のサンプル MOD です。MOD API で MOD を書くときの見本になります。

- **エディタの MOD 欄から**（どのブラウザでも、GitHub Pages などのサイト・アプリ・スマホでも）：「URLから追加」に
  `https://raw.githubusercontent.com/qwaxgo/ODM-Poser-SampleMods/main/hello_mod.js` を入れる（毎回新しい版を読みます）。
  または `hello_mod.js` をダウンロードして「ファイルから入れる」。
- **フォルダから開くエディタで**：エディタの `mods/` にこのリポジトリを clone し、エディタのフォルダで
  `python tools/make_mods_list.py` を実行してから開き直す。
- **ComfyUI で**（ODM-Poser-ComfyUIBridge を入れている場合）：ブリッジの `mods/` にこのリポジトリを clone して、エディタを開き直す。

MOD を一時的に止めるには、名前の頭に `_` を付けるか、MOD 欄で無効にします。

## Built with Claude Code / Claude Code での実装

The code and documents of this repository were implemented by [Claude Code](https://claude.com/claude-code),
Anthropic's AI coding tool, under qwaxgo's design and direction.
このリポジトリのコードとドキュメントは、qwaxgo の設計と指示のもとで、Anthropic の AI コーディングツール Claude Code が実装しました。

## License

MIT, (c) 2026 qwaxgo. See `LICENSE`.
