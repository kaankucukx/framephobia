<p align="center">
  <img src="icon.png" width="96" alt="Framephobia logo">
</p>

<h1 align="center">Framephobia</h1>

<p align="center">
  A high-contrast dark theme for VS Code, tuned for component-driven front-end code.
</p>

<p align="center">
  <a href="https://marketplace.visualstudio.com/items?itemName=kaankucuk.framephobia"><img src="https://vsmarketplacebadges.dev/version-short/kaankucuk.framephobia.svg?style=flat-square&color=8146FE&label=marketplace" alt="Marketplace version"></a>
  <a href="https://marketplace.visualstudio.com/items?itemName=kaankucuk.framephobia"><img src="https://vsmarketplacebadges.dev/installs-short/kaankucuk.framephobia.svg?style=flat-square&color=23EBD0&label=installs" alt="Installs"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-FFCC00?style=flat-square" alt="MIT license"></a>
</p>

![Framephobia preview](https://user-images.githubusercontent.com/20001862/49329267-0487c280-f58d-11e8-8077-845549dc86b7.png)

## Why

Most dark themes treat a `.vue` template or an Angular component as plain HTML. Framephobia does not. Custom components, framework directives and unrecognized attributes each get their own color, so the structure of a template reads at a glance and the framework layer stands apart from the markup it decorates.

## Highlights

| Area | Treatment |
| --- | --- |
| Custom components | `<my-card>`, `<app-root>` and Vue component tags in violet `#8146FE` |
| Directives and bindings | Vue `:prop`, `@event`, `v-if` in teal `#23EBD0` |
| Unrecognized attributes | Angular `fxFlex`-style attributes in yellow `#FFCC00` |
| Native HTML | Plain tags and class strings stay muted so components stand out |
| Doc comments | JSDoc tags and types faded to 25% opacity, present but quiet |
| TypeScript | Distinct colors for interfaces, primitive types, `this` and constants |
| Workbench | Bracket pair colors, git decorations, terminal ANSI and panels all use the same palette |

Also covers JavaScript, TypeScript, HTML, CSS/SCSS/Less, JSON, Markdown, Python, PHP, Java, C/C++, C#, Go and Elm.

## Palette

| Role | Color |
| --- | --- |
| Background | `#19191f` |
| Components, storage types | `#8146FE` |
| Directives, active tab, accents | `#23EBD0` |
| Cursor, block braces | `#FFCC00` |
| Keywords | `#D55FDE` |
| Functions | `#52ADF2` |
| Variables | `#EF596F` |
| Strings | `#89CA78` |
| Numbers, constants | `#D8985F` |
| Operators | `#2BBAC5` |
| Comments | `#826f49` |

## Install

From VS Code: open Extensions (`Cmd+Shift+X` / `Ctrl+Shift+X`), search **Framephobia**, install, then pick it under **Preferences: Color Theme**.

From the command line:

```bash
code --install-extension kaankucuk.framephobia
```

## Recommended settings

Framephobia colors TypeScript through TextMate scopes and ships with semantic highlighting turned off so the template and directive colors stay consistent. Bracket pair colors come from the theme palette.

```jsonc
{
  "workbench.colorTheme": "Framephobia",
  "editor.bracketPairColorization.enabled": true,
  "editor.fontLigatures": true
}
```

## The name

Framephobia started during a job switch from a Vue codebase to an Angular one: TypeScript, RxJS, NgRx, Jasmine and Karma all at once. Recoloring the editor between those sessions turned into this theme. The name is the framework anxiety it came out of.

## Contributing

Issues and pull requests are welcome. To try changes locally, open the repository in VS Code and press `F5` to launch an Extension Development Host with the theme loaded. `Developer: Inspect Editor Tokens and Scopes` shows which scope a token resolves to.

## License

[MIT](LICENSE)
