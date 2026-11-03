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
- **The HTML release** (the zip from the editor's GitHub Releases, opened from disk): clone this
  repository into the `mods/` folder next to `index.html`, then either press **From a folder** in
  the MOD panel and pick that `mods/` folder (Chrome and Edge remember it), or add the line
  `"ODM-Poser-SampleMods/hello_mod.js",` to `mods.js` next to it, and reload.
  ```
  cd ODM-Poser-v0.1.0/mods
  git clone https://github.com/qwaxgo/ODM-Poser-SampleMods
  ```
- **The app** (AppImage, Windows zip): clone this repository into the `mods/` folder next to the
  executable and restart the app.
- **Working on the editor** (`npm run dev` in a checkout of ODM-Poser): clone this repository into
  the checkout's `mods/` folder, run `python tools/make_mods_list.py` there and reload.
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
- **HTML 版で**（エディタの GitHub Releases の zip をディスクから開く場合）：`index.html` の隣の `mods/` にこのリポジトリを clone します。
  そのあと次のどちらかをして、開き直します。
  - MOD 欄の「フォルダから」でその `mods/` を選ぶ（Chrome と Edge はフォルダを覚えます）
  - 隣の `mods.js` に `"ODM-Poser-SampleMods/hello_mod.js",` の1行を足す
- **アプリ版で**（AppImage、Windows の zip）：実行ファイルの隣の `mods/` にこのリポジトリを clone して、アプリを起動し直す。
- **エディタを手直しするとき**（ODM-Poser を clone して `npm run dev`）：その `mods/` にこのリポジトリを clone し、
  そのフォルダで `python tools/make_mods_list.py` を実行してから開き直す。
- **ComfyUI で**（ODM-Poser-ComfyUIBridge を入れている場合）：ブリッジの `mods/` にこのリポジトリを clone して、エディタを開き直す。

MOD を一時的に止めるには、名前の頭に `_` を付けるか、MOD 欄で無効にします。

## Built with Claude Code / Claude Code での実装

The code and documents of this repository were implemented by [Claude Code](https://claude.com/claude-code),
Anthropic's AI coding tool, under qwaxgo's design and direction.
このリポジトリのコードとドキュメントは、qwaxgo の設計と指示のもとで、Anthropic の AI コーディングツール Claude Code が実装しました。

## License

MIT, (c) 2026 qwaxgo. See `LICENSE`.
