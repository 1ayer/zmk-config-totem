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
- Added all combos from original main keymap in `config/totem.keymap`:
  - `wr` (`<3 1>` -> `RIGHT_ALT`)
  - `xv` (`<24 22>` -> `RCTRL`)
  - `uo` (`<6 8>` -> `RIGHT_ALT`)
  - `mdot` (`<27 29>` -> `RCTRL`)

## Commit C - Add Custom Behaviors

Enabled:
- Added custom hold-tap behavior definitions in `config/totem.keymap`:
  - `nlt`
  - `nmt`
- No per-layer binding changes in this commit
