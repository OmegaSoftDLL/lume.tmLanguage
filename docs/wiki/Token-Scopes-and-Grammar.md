<h1>
  <img src="https://raw.githubusercontent.com/OmegaSoftDLL/lume.tmLanguage/main/docs/assets/lume-mascot-badge.svg" alt="Lumi" width="76" height="76" align="left" />
  Token Scopes &amp; Grammar Reference (<code>source.lume</code>)
</h1>
<br clear="left"/>

`syntaxes/Lume.tmLanguage.json` defines the canonical root scope `source.lume` for `.lume` and `.src` files.

## Primary Scope Hierarchy

| Scope Name | Pattern / Tokens |
| :--- | :--- |
| `comment.block.lume` | Nested `#[ ... ]#` block comments |
| `comment.line.documentation.lume` | `## ...` documentation comments |
| `comment.line.number-sign.lume` | `# ...` single-line comments |
| `meta.attribute.lume` / `entity.name.attribute.lume` | `@secret`, `@bound`, `@inline`, `@cold` |
| `meta.effect.lume` / `storage.modifier.effect.lume` | `/ pure`, `/ {io, net, ffi}` |
| `storage.modifier.verification.lume` | `requires`, `ensures`, `invariant`, `law`, `verify` |
| `storage.type.lume` | `fn`, `type`, `record`, `enum`, `error`, `trait`, `impl`, `const`, `mod`, `use`, `extern`, `effect`, `model`, `macro` |
| `storage.modifier.lume` | `pub`, `crate`, `own`, `mut`, `unsafe`, `total`, `par` |
| `keyword.control.lume` | `if`, `then`, `elif`, `else`, `match`, `with`, `handler`, `resume`, `for`, `while`, `loop`, `in`, `return`, `defer`, `spawn`, `select` |
| `entity.name.function.lume` | Function identifier in `fn <identifier>` |
| `storage.type.primitive.lume` | `bool`, `char`, `str`, `int`, `uint`, `float`, `decimal`, `i8`..`i128`, `u8`..`u128`, `f16`..`f64`, `never`, `Self` |
| `entity.name.type.lume` | Uppercase ADT constructors & type identifiers (`Cons`, `Nil`, `Option`, `Result`) |
| `string.quoted.double.lume` / `meta.interpolation.lume` | `"..."` strings with `{...}` interpolation and `{{`/`}}` escaped braces |
| `constant.numeric.lume` | Decimal, hexadecimal (`0x`), binary (`0b`), octal (`0o`), and scientific floats |
| `keyword.operator.lume` | `\|>`, `->`, `=>`, `+%`, `-%`, `*%`, `==`, `!=`, `<=`, `>=` |
