# media-sound/audacity

## PR 35903 HEAD 911aff1

__LXC container__: _Gentoo amd64 (openrc) (20240408_16:07) container_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#911aff1](https://github.com/Jamim/gentoo/tree/911aff12f7fe07a527a7faa15c78156b1a15b8f7)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)

### media-sound/audacity-3.3.3-r1

__SUCCESS__

USE="-* vamp" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```
