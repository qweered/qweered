<h1 align="center">Aliaksandr</h1>

<p align="center">
  <i>Software engineer · Vilnius, Lithuania</i>
</p>

<p align="center">
  Open-source contributor focused on the <a href="https://nixos.org">Nix ecosystem</a> — <strong>~100 merged PRs to <a href="https://github.com/NixOS/nixpkgs">nixpkgs</a></strong> in the last year.
</p>

<p align="center">
  <a href="https://github.com/qweered">
    <img src="https://github-readme-stats.vercel.app/api?username=qweered&count_private=true&show_icons=true&theme=github_dark&hide_border=true&hide_title=true" alt="GitHub stats" />
  </a>
  <a href="https://github.com/qweered">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=qweered&theme=github_dark&hide_border=true&layout=compact&hide=html,css" alt="Top languages" />
  </a>
</p>

### What I work on

| Area | Focus |
|------|-------|
| **Nix / NixOS** | nixpkgs packaging, infrastructure, CI tooling, performance, treewide refactors |
| **Developer tooling** | flatpak, Hyprland on NixOS |
| **Frontend** | React, TypeScript, Expo (side projects) |

### Selected open-source contributions (past year)

#### nixpkgs

- **`fetchPnpmDeps` v1 → v3 migration** — multi-part treewide migration of pnpm-based packages: [part 1](https://github.com/NixOS/nixpkgs/pull/494210) · [part 2](https://github.com/NixOS/nixpkgs/pull/494400) · [part 3](https://github.com/NixOS/nixpkgs/pull/494401) · [part 4](https://github.com/NixOS/nixpkgs/pull/494402), and a [v1 deprecation proposal](https://github.com/NixOS/nixpkgs/pull/513215)
- [**`pipewire` 1.4 → 1.6**](https://github.com/NixOS/nixpkgs/pull/492490) — major update; moved pipewire and wireplumber to `by-name`, modernized
- [**`sddm-astronaut` refactor**](https://github.com/NixOS/nixpkgs/pull/492325) — closure-size reductions; co-maintainer
- **Performance**: [`patch-shebangs`: optimize bash + add ANSI C implementation](https://github.com/NixOS/nixpkgs/pull/482713) · [reduce `//` merges and optimize `++` chains across hot paths](https://github.com/NixOS/nixpkgs/pull/506793) · [stdenv: `// optionalAttrs` → nullable attr names](https://github.com/NixOS/nixpkgs/pull/506774) · [`lib/attrsets`: use `builtins.filterAttrs` when available](https://github.com/NixOS/nixpkgs/pull/498999)
- **CI / merge bot**: [auto-label new and updated packages](https://github.com/NixOS/nixpkgs/pull/482478) · [surface auto-merge blockers in the bot's checklist](https://github.com/NixOS/nixpkgs/pull/513224) · gating on `no PR failures` and committer change-requests
- **Hardening**: [assert no `by-name` overwrites](https://github.com/NixOS/nixpkgs/pull/483820) · [no `callPackage` with by-name paths](https://github.com/NixOS/nixpkgs/pull/489120) · [progressively extend by-name defaults](https://github.com/NixOS/nixpkgs/pull/483378)
- **New packages**: [`crosspipe`](https://github.com/NixOS/nixpkgs/pull/494512) · [`volt`](https://github.com/NixOS/nixpkgs/pull/492342) · [`nix-olde`](https://github.com/NixOS/nixpkgs/pull/492280) · [`vite-plus`](https://github.com/NixOS/nixpkgs/pull/500492)
- **Treewide cleanups**: `meta = with lib;` removal, `rec` → `finalAttrs`, ~20 PRs moving overrides into `package.nix`, qt6 application moves to by-name, override consolidation across audacity / bitwuzla / cvc5 / hugin / mysql-workbench / neovim-unwrapped / plausible / rabbitmq-server and more

### Elsewhere

- [**hyprnixos**](https://github.com/qweered/hyprnixos) — full NixOS + Hyprland configuration
- [**automaspec**](https://github.com/qweered/automaspec) — pair project: AI-assisted platform that turns requirements into test specs and generated test code (Next.js 16, ORPC, Drizzle, multi-tenant)
- [**expo-shizuku**](https://github.com/qweered/expo-shizuku) — Expo native module for silent APK installation via Shizuku on Android
- [**flatpak**](https://github.com/flatpak/flatpak/pull/6635) — fish profile fast-path skip when `XDG_DATA_DIRS` already includes the path
