__THIS REPO IS SUBJECT TO FORCED PUSH__

# media-sound/audacity

## PR 35903 HEAD 911aff1

Summary of [512e17d..911aff1](https://github.com/gentoo/gentoo/compare/512e17d21024862b7e2f58025fe72354863ee345..911aff12f7fe07a527a7faa15c78156b1a15b8f7), see also [35903#issuecomment-2050869857](https://github.com/gentoo/gentoo/pull/35903#issuecomment-2050869857):
- fix compiling failure of [PR 35903 HEAD 512e17d 3.3.3-r1 iteration #2](#user-content-failure-pr-35903-head-512e17d-3.3.3-r1-2).

__LXC container__: _Gentoo amd64 (openrc) (20240408_16:07) container_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#911aff1](https://github.com/Jamim/gentoo/tree/911aff12f7fe07a527a7faa15c78156b1a15b8f7)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)

### <a id="pr-35903-head-911aff1-3.3.3-r1" />media-sound/audacity-3.3.3-r1

Resume from [PR 35903 HEAD 512e17d](#user-content-pr-35903-head-512e17d-3.3.3-r1).

__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/7/)__

USE="-* ogg opus" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

## PR 35903 HEAD 512e17d

Resume from [PR 35903 HEAD 05d838a](#user-content-pr-35903-head-05d838a).

Summary of [05d838a..512e17d](https://github.com/gentoo/gentoo/compare/05d838a28b1c2516741f7ff25b2c4e89984e76e8..512e17d21024862b7e2f58025fe72354863ee345), see also [35903#issue-2204604236](https://github.com/gentoo/gentoo/pull/35903#issue-2204604236):
- fix missing `#include <limits>` for `2.4.2-r3`
- limit `media-video/ffmpeg` to `<5` for `2.4.2-r3`
- add `x11-base/xorg-proto` to `DEPEND` <sup>[1]</sup>
- add ASM to `BDEPEND` <sup>[1]</sup>

1. fix compiling failure of [PR 35903 HEAD 05d838a 3.4.2-r1 iteration #2](#user-content-failure-pr-35903-head-05d838a-3.4.2-r1-2).

__LXC container__: _Gentoo amd64 (openrc) (20240408_16:07) container_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#512e17d](https://github.com/Jamim/gentoo/tree/512e17d21024862b7e2f58025fe72354863ee345)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)

### media-sound/audacity-3.4.2-r1

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/4/)__

USE="-*" ABI_X86="(64)"

```
emerge =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/5/)__

USE="-*" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/6/)__

USE="-* audiocom" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/7/)__

USE="-* flac" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/8/)__

USE="-* lv2" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/9/)__

USE="-* ogg" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/10/)__

USE="-* ogg opus" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/11/)__

USE="-* ogg vorbis" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/12/)__

USE="-* ladspa" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/13/)__

USE="-* mpg123" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/14/)__

USE="-* twolame" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/15/)__

USE="-* vamp" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/16/)__

USE="-* wavpack" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/17/)__

USE="-* ffmpeg" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/18/)__

USE="-* portmixer" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/19/)__

USE="-* sbsms" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/20/)__

USE="-* id3tag" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/21/)__

USE="-* alsa" ABI_X86="(64)"

PS: media-sound/audacity[alsa] requires media-libs/portaudio[alsa].

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/22/)__

USE="* -test" ABI_X86="(64)"

PS: The '*' here is a non-functional pseudo wildcard, meaning all;
    media-sound/audacity[alsa] requires media-libs/portaudio[alsa].

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/23/)__

USE="*" ABI_X86="(64)"

PS: The '*' here is a non-functional pseudo wildcard, meaning all;
    media-sound/audacity[alsa] requires media-libs/portaudio[alsa];
    media-sound/audacity[test] requires x11-base/xorg-server[xvfb].

NOTES: To run the tests (aka USE="test" and FEATURES="test"), don't
       mount /tmp/.X11-unix in the LXC container, Xvfb requires the
       /tmp/.X11-unix directory to be owned by the LXC container.

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

### <a id="pr-35903-head-512e17d-3.3.3-r1" />media-sound/audacity-3.3.3-r1

Continue in [PR 35903 HEAD 911aff1](#user-content-pr-35903-head-911aff1-3.3.3-r1).

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/1/)__

USE="-*" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="failure-pr-35903-head-512e17d-3.3.3-r1-2" />__[FAILURE](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/2/)__

Fixed in [PR 35903 HEAD 911aff1](#user-content-pr-35903-head-911aff1).

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

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/3/)__

USE="-* audiocom" ABI_X86="(64)"

Applied audacity-3.4.2-audiocom-std-string.patch from PR 35414.

References:
- [bug#920363](https://bugs.gentoo.org/920363)
- [gentoo/gentoo#35414](https://github.com/gentoo/gentoo/pull/35414)

Resume from [PR 35903 HEAD 512e17d 3.3.3-r1 iteration #2](#user-content-failure-pr-35903-head-512e17d-3.3.3-r1-2), after the aforementioned patch.

```
emerge =media-sound/audacity-3.3.3-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/4/)__

USE="-* flac" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/5/)__

USE="-* lv2" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/6/)__

USE="-* ogg" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

## PR 35903 HEAD 05d838a

All tests here are redone in [PR 35903 HEAD 512e17d](#user-content-pr-35903-head-512e17d).

__LXC container__: _Gentoo amd64 (openrc) (20240406_16:07)_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#05d838a](https://github.com/Jamim/gentoo/tree/05d838a28b1c2516741f7ff25b2c4e89984e76e8)  
Head of Gentoo's repo: [gentoo/gentoo#be766b5](https://github.com/gentoo/gentoo/tree/be766b5b349fc88b7c91c35074560d162240c3fd)

### media-sound/audacity-3.4.2-r1

__[SUCCESS](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r1/1/)__

USE="-*" ABI_X86="(64)"

```
emerge =media-sound/audacity-3.4.2-r1
```

<a id="failure-pr-35903-head-05d838a-3.4.2-r1-2" />__[FAILURE](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r1/2/)__

Fixed in [PR 35903 HEAD 512e17d](#user-content-pr-35903-head-512e17d).

USE="-*" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

### media-sound/audacity-3.4.2-r2

__[SUCCESS](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r2/3/)__

Applied suggested [patch](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r2/3/audacity-3.4.2-r2-3.patch) to fix [PR 35903 HEAD 05d838a 3.4.2-r1 iteration #2](#user-content-failure-pr-35903-head-05d838a-3.4.2-r1-2).

USE="-*" ABI_X86="(64)"

```
cd /var/db/repos/localrepo/media-sound/audacity
cp audacity-3.4.2-r{1,2}.ebuild
patch -p1 < .../audacity-3.4.2-r2-3.patch
ebuild audacity-3.4.2-r2.ebuild manifest
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r2 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r2-*
emerge -k =media-sound/audacity-3.4.2-r2
```
