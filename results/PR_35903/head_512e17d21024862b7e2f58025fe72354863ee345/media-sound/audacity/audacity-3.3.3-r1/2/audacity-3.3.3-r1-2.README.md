# media-sound/audacity

__LXC container__: _Gentoo amd64 (openrc) (20240408_16:07) container_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#512e17d](https://github.com/Jamim/gentoo/tree/512e17d21024862b7e2f58025fe72354863ee345)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)

## media-sound/audacity-3.3.3-r1

__FAILURE__

USE="-* audiocom" ABI_X86="(64)"

Requires audacity-3.4.2-audiocom-std-string.patch from PR 35414, which
was not included into media-sound/audacity-3.3.3 ebuild after merging.

References:
- [bug#920363](https://bugs.gentoo.org/920363)
- [gentoo/gentoo#35414](https://github.com/gentoo/gentoo/pull/35414)

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```
