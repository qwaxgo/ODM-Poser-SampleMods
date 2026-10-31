# ODM-Poser-SampleMods — notes for AI coding agents

The editor's UI follows **melta UI** (`design/melta-ui`, a git submodule; read
`design/melta-ui/DESIGN.md`). A mod's panel (`api.ui.addSection`) gets melta's look from the editor
(its `web/editor/ui.js`) by what each control is, in light and dark:

- write plain markup: `section > h2` is made by addSection; inside it use `label`, `button`
  (`class="primary"` for the one main action), `select`, `input`, `class="hint"` for notes, and
  `class="row"`, `"btns"`, `"grid2"` for layout;
- do not give controls colours, borders, paddings or fonts (inline styles or a stylesheet): they
  would break melta's look and the dark theme;
- pictures drawn on the canvas (props, auras, the `draw` hook) are the pose's content, not the UI:
  they keep their own colours.
