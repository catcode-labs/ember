# Ember
**Ember** is the developer companion CLI for the [Anvil](https://github.com/catcode-labs/anvil) package manager ecosystem.

It streamlines local development, dry-run testing, manifest linting, and workspace security sealing for software maintainers.

---

## Features

* **Scaffold Blueprints:** Generate annotated `.ember` draft files with `ember light`.
* **Linting & Validation:** Validate TOML syntax, rules, and host system dependencies with `ember inspect`.
* **Atomic Testing & Sealing:** Execute dry-run builds, verify target binary outputs, compute master SHA-256 sidecars, and stage releases using `ember ignite`.
* **Workspace Housekeeping:** Easily clean intermediate build junk (`ember douse`) or un-seal security sidecars (`ember extinguish`).

---

## Installation

```
cargo install --git https://github.com/catcode-labs/ember
```

---

## Usage


1. Create a new blueprint in current directory
```
ember light projectname
```
2. Validate syntax and host dependencies
```
ember inspect projectname.ember
```
3. Test build, generate .anvil & .anvil.sha256, and push to GitHub
```
ember ignite projectname.ember --push
```
Aliases are available for all commands (init, check, seal, clean, reset)
```
ember check projectname.ember
```


---

## 📄 License

**Ember** is part of **CatCode Labs** and is licensed under the **GNU General Public License v3.0** (GPL-3.0-or-later).
See the [LICENSE](LICENSE) for the full license text.
