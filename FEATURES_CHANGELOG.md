# Feature Enablement Changelog

This file tracks incremental feature reintroduction after the minimal baseline.

## Commit A - Add Layers Only

Enabled:
- Added additional layers using original(main) keybindings:
  - `num_layer`
  - `func_layer`
  - `nav_layer`
  - `sym_layer`
  - `device_layer`
- No combos, custom behaviors, Studio, or mouse keys added in this commit.

## Commit B - Add Small Combo Set

Enabled:
- Added one combo (`wr_combo`) in `config/totem.keymap`
- Binding: key positions `<3 1>` -> `RIGHT_ALT`
- Scope kept minimal to reduce compile risk
