<h1>
  <img src="https://raw.githubusercontent.com/OmegaSoftDLL/lume.tmLanguage/main/docs/assets/lume-mascot-badge.svg" alt="Lumi" width="76" height="76" align="left" />
  Editor Integration Guide (VS Code, Zed, Sublime, Neovim)
</h1>
<br clear="left"/>

## 1. VS Code / Cursor / VSCodium

```bash
git clone https://github.com/OmegaSoftDLL/lume.tmLanguage.git ~/.vscode/extensions/omegasoftdll.lume-tmlanguage-1.1.0
```

## 2. Sublime Text 4

Copy `syntaxes/Lume.tmLanguage.json` into your Sublime `Packages/User/` folder.

## 3. TextMate 2 &amp; Neovim (`nvim-treesitter` / `vim-textmate`)

Point your TextMate grammar loader to `syntaxes/Lume.tmLanguage.json` for `*.lume` and `*.src` buffers, and attach `lume lsp` as your stdio Language Server:

```lua
vim.lsp.start({
  name = "lume-lsp",
  cmd = { "lume", "lsp" },
  root_dir = vim.fn.getcwd(),
})
```
