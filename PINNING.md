# ZMK Version Pinning

This branch pins ZMK in `config/west.yml` to `v0.3.0` for reproducible builds.

## Update Procedure

1. Choose a tested ZMK release tag (or specific commit SHA).
2. Edit `config/west.yml` and change `revision:` under the `zmk` project.
3. Rebuild both halves (`totem_left`, `totem_right`) and `settings_reset`.
4. Flash both halves and verify split + USB input.
5. Commit with a message like `chore: bump zmk pin to <tag-or-sha>`.
