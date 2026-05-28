# Patches: ubuntu resolute / loong64

Add .patch files here for ubuntu-specific kernel patches targeting resolute.
List them in `series` (one filename per line, quilt format).

Consumer support: xanmod ✓ liquorix — liqxanmod —

## Adding a patch

1. Create `NNN-description.patch` in this directory
2. Add the filename to `series`
3. Commit and push

The build system applies patches in `series` order after the arch base
patches and before the patchset (XanMod/Liquorix) patches.
