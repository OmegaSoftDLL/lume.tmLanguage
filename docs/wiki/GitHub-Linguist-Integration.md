<h1>
  <img src="https://raw.githubusercontent.com/OmegaSoftDLL/lume.tmLanguage/main/docs/assets/lume-mascot-badge.svg" alt="Lumi" width="76" height="76" align="left" />
  GitHub Linguist Integration
</h1>
<br clear="left"/>

Add the following rules to `.gitattributes` at the root of any Lume project so GitHub Linguist recognizes `.lume` and `.src` files as **Lume**:

```gitattributes
*.lume text eol=lf linguist-language=Lume
*.src  text eol=lf linguist-language=Lume
```
