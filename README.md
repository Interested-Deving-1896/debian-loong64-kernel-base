# debian-loong64-kernel-base

Authoritative kernel base for **loong64** across Debian, Devuan, and Ubuntu.

Pins kernel `v6.9` from [kernel.org](https://cdn.kernel.org/pub/linux/kernel/v6.x/linux-6.9.tar.xz).
Devuan and Ubuntu patches live as branches here — they are downstream
derivatives of Debian, not separate source trees.

## Branch structure

```
main                          kernel version pin (this branch)
patchset/debian/trixie        Debian trixie config + patches
patchset/debian/forky         Debian forky
patchset/debian/sid           Debian sid (unstable)
patchset/devuan/excalibur     Devuan excalibur (no-systemd delta)
patchset/devuan/forky         Devuan forky
patchset/devuan/ceres         Devuan ceres (unstable)
patchset/ubuntu/resolute      Ubuntu resolute config + patches
patchset/ubuntu/stonking      Ubuntu stonking
patchset/ubuntu/devel         Ubuntu devel
```

## Consumers

- [xanmod-unified-kernel](https://github.com/Interested-Deving-1896/xanmod-unified-kernel)
- [liquorix-unified-kernel](https://github.com/Interested-Deving-1896/liquorix-unified-kernel)
- [liqxanmod](https://github.com/Interested-Deving-1896/liqxanmod)

## Updating the kernel version

Edit `VERSION` and `READY` on `main`. Consumers pick up the new version
on their next build automatically.
