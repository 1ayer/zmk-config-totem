# Baseline Profile (Minimal Stable Split)

This repository is currently set to a minimal baseline intended to reduce RAM/stack pressure while keeping split operation intact (`totem_left` / `totem_right`).

## What is temporarily disabled

- ZMK Studio build snippet in `build.yaml`
- ZMK Studio Kconfig options in `config/totem.conf`
- Heavy keymap constructs in `config/totem.keymap`:
  - combos
  - custom hold-tap behaviors
  - macros
  - extra layers beyond two layers

## Incremental re-enable checklist

1. Build and flash this baseline on both halves and verify typing + LOWER layer.
2. Re-enable Studio only:
   - Uncomment `CONFIG_ZMK_STUDIO=y` in `config/totem.conf`
   - Add `snippet: studio-rpc-usb-uart` back to `totem_left` in `build.yaml`
3. Add one advanced behavior at a time (recommended order):
   - hold-tap
   - combos
   - macros
4. Add additional layers (3rd layer+) one by one.
5. After each step, rebuild and test both halves before continuing.
