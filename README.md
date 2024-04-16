__THIS REPO IS SUBJECT TO FORCED PUSH__

# media-sound/audacity

__NOTES:__

1. <a id="main-note-1" />Will later use `media-libs/libsndfile[minimal]` to not install dependencies beyond `media-sound/audacity` strict
   requirements ([`media-sound/audacity-2.4.2-r3[doc]: PR 35903 HEAD 911aff1 SUCCESS`](#user-content-success-pr-35903-head-911aff1-2.4.2-r3-7)).

## PR 35903 HEAD 911aff1

Summary of [512e17d..911aff1](https://github.com/gentoo/gentoo/compare/512e17d21024862b7e2f58025fe72354863ee345..911aff12f7fe07a527a7faa15c78156b1a15b8f7), see also [35903#issuecomment-2050869857](https://github.com/gentoo/gentoo/pull/35903#issuecomment-2050869857):
- fix compiling failure of [PR 35903 HEAD 512e17d 3.3.3-r1 iteration #2](#user-content-failure-pr-35903-head-512e17d-3.3.3-r1-2).

__LXC container__: _Gentoo amd64 (openrc) (20240408_16:07) container_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#911aff1](https://github.com/Jamim/gentoo/tree/911aff12f7fe07a527a7faa15c78156b1a15b8f7)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)

### <a id="pr-35903-head-911aff1-2.4.2-r3" />media-sound/audacity-2.4.2-r3

- <a id="failure-pr-35903-head-911aff1-2.4.2-r3-1" />[`media-sound/audacity-2.4.2-r3[-*]: PR 35903 HEAD 911aff1 FAILURE`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/1/)

  Undefined references about `libflac`, required by Audacity's ondemand
  (aka OD) file handling, even when `libflac` support had been disabled
  via configure.

  Triggers: [bug#741969](https://bugs.gentoo.org/741969)  
  Triggers: [bug#884747](https://bugs.gentoo.org/884747)

  Fixed in [`media-sound/audacity-2.4.2-r3[-*]: PR 35903 HEAD 911aff1 SUCCESS (patch)`](#user-content-success-pr-35903-head-911aff1-2.4.2-r3-2)
  via suggested patch.

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-2" />[`media-sound/audacity-2.4.2-r3[-*]: PR 35903 HEAD 911aff1 SUCCESS (patch)`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/2/)

  Fixes [`media-sound/audacity-2.4.2-r3[-*]: PR 35903 HEAD 911aff1 FAILURE`](#user-content-failure-pr-35903-head-911aff1-2.4.2-r3-1)
  via suggested [audacity-2.4.2-fix-libflac-undefined-references.patch](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/2/files/audacity-2.4.2-fix-libflac-undefined-references.patch).

  Closes: [bug#741969](https://bugs.gentoo.org/741969)  
  Closes: [bug#884747](https://bugs.gentoo.org/884747)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-3" />[`media-sound/audacity-2.4.2-r3[flac]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/3/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-4" />[`media-sound/audacity-2.4.2-r3[lv2]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/4/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-5" />[`media-sound/audacity-2.4.2-r3[ogg]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/5/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-6" />[`media-sound/audacity-2.4.2-r3[vorbis]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/6/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-7" />[`media-sound/audacity-2.4.2-r3[doc]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/7/)

  _FROM HERE ON <sup>[[main note 1]](#user-content-main-note-1)</sup>_

  Use `media-libs/libsndfile[minimal]` to not install dependencies
  beyond `media-sound/audacity` strict requirements.

  `media-libs/libsndfile-1.2.2-r2[!minimal]` would install:
  - `media-libs/flac`
  - `media-libs/libogg`
  - `media-libs/libvorbis`
  - `media-libs/opus`
  - `media-sound/lame`
  - `media-sound/mpg123-base`

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-8" />[`media-sound/audacity-2.4.2-r3[jack]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/8/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-9" />[`media-sound/audacity-2.4.2-r3[vst]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/9/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-10" />[`media-sound/audacity-2.4.2-r3[ladspa]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/10/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-11" />[`media-sound/audacity-2.4.2-r3[mad]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/11/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-12" />[`media-sound/audacity-2.4.2-r3[twolame]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/12/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-13" />[`media-sound/audacity-2.4.2-r3[vamp]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/13/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-14" />[`media-sound/audacity-2.4.2-r3[ffmpeg]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/14/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-15" />[`media-sound/audacity-2.4.2-r3[oss]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/15/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-16" />[`media-sound/audacity-2.4.2-r3[portmidi,portsmf]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/16/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-17" />[`media-sound/audacity-2.4.2-r3[portmixer]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/17/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-18" />[`media-sound/audacity-2.4.2-r3[portsmf]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/18/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-19" />[`media-sound/audacity-2.4.2-r3[sbsms]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/19/)

- <a id="success-pr-35903-head-911aff1-2.4.2-r3-20" />[`media-sound/audacity-2.4.2-r3[id3tag]: PR 35903 HEAD 911aff1 SUCCESS`](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-2.4.2-r3/20/)

### <a id="pr-35903-head-911aff1-3.3.3-r1" />media-sound/audacity-3.3.3-r1

Resume from [PR 35903 HEAD 512e17d](#user-content-pr-35903-head-512e17d-3.3.3-r1).

<a id="success-pr-35903-head-911aff1-3.3.3-r1-7" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/7/)__

USE="-* ogg opus" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-8" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/8/)__

USE="-* ogg vorbis" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-9" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/9/)__

USE="-* ladspa" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-10" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/10/)__

USE="-* mpg123" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-11" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/11/)__

USE="-* twolame" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-12" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/12/)__

USE="-* vamp" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-13" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/13/)__

USE="-* wavpack" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-14" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/14/)__

USE="-* ffmpeg" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-15" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/15/)__

USE="-* portmixer" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-16" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/16/)__

USE="-* sbsms" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-17" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/17/)__

USE="-* id3tag" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-18" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/18/)__

USE="-* alsa" ABI_X86="(64)"

PS: media-sound/audacity[alsa] requires media-libs/portaudio[alsa].

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-19" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/19/)__

USE="-* mad" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-20" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/20/)__

USE="* -mpg123 -test" ABI_X86="(64)"

PS: The '*' here is a non-functional pseudo wildcard, meaning all;
    media-sound/audacity[alsa] requires media-libs/portaudio[alsa].

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-21" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/21/)__

USE="* -mad -test" ABI_X86="(64)"

PS: The '*' here is a non-functional pseudo wildcard, meaning all;
    media-sound/audacity[alsa] requires media-libs/portaudio[alsa].

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-22" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/22/)__

USE="* -mpg123" ABI_X86="(64)"

PS: The '*' here is a non-functional pseudo wildcard, meaning all;
    media-sound/audacity[alsa] requires media-libs/portaudio[alsa];
    media-sound/audacity[test] requires x11-base/xorg-server[xvfb].

NOTES: To run the tests (aka USE="test" and FEATURES="test"), don't
       mount /tmp/.X11-unix in the LXC container, Xvfb requires the
       /tmp/.X11-unix directory to be owned by the LXC container.

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-911aff1-3.3.3-r1-23" />__[SUCCESS](results/PR_35903/head_911aff12f7fe07a527a7faa15c78156b1a15b8f7/media-sound/audacity/audacity-3.3.3-r1/23/)__

USE="* -mad" ABI_X86="(64)"

PS: The '*' here is a non-functional pseudo wildcard, meaning all;
    media-sound/audacity[alsa] requires media-libs/portaudio[alsa];
    media-sound/audacity[test] requires x11-base/xorg-server[xvfb].

NOTES: To run the tests (aka USE="test" and FEATURES="test"), don't
       mount /tmp/.X11-unix in the LXC container, Xvfb requires the
       /tmp/.X11-unix directory to be owned by the LXC container.

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

### <a id="pr-35903-head-512e17d-3.4.2-r1" />media-sound/audacity-3.4.2-r1

<a id="success-pr-35903-head-512e17d-3.4.2-r1-4" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/4/)__

USE="-*" ABI_X86="(64)"

```
emerge =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-5" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/5/)__

USE="-*" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-6" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/6/)__

USE="-* audiocom" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-7" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/7/)__

USE="-* flac" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-8" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/8/)__

USE="-* lv2" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-9" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/9/)__

USE="-* ogg" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-10" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/10/)__

USE="-* ogg opus" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-11" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/11/)__

USE="-* ogg vorbis" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-12" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/12/)__

USE="-* ladspa" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-13" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/13/)__

USE="-* mpg123" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-14" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/14/)__

USE="-* twolame" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-15" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/15/)__

USE="-* vamp" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-16" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/16/)__

USE="-* wavpack" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-17" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/17/)__

USE="-* ffmpeg" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-18" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/18/)__

USE="-* portmixer" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-19" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/19/)__

USE="-* sbsms" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-20" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/20/)__

USE="-* id3tag" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-21" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/21/)__

USE="-* alsa" ABI_X86="(64)"

PS: media-sound/audacity[alsa] requires media-libs/portaudio[alsa].

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

<a id="success-pr-35903-head-512e17d-3.4.2-r1-22" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/22/)__

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

<a id="success-pr-35903-head-512e17d-3.4.2-r1-23" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.4.2-r1/23/)__

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

<a id="success-pr-35903-head-512e17d-3.3.3-r1-1" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/1/)__

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

<a id="success-pr-35903-head-512e17d-3.3.3-r1-3" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/3/)__

USE="-* audiocom" ABI_X86="(64)"

Applied audacity-3.4.2-audiocom-std-string.patch from PR 35414.

References:
- [bug#920363](https://bugs.gentoo.org/920363)
- [gentoo/gentoo#35414](https://github.com/gentoo/gentoo/pull/35414)

Resume from [PR 35903 HEAD 512e17d 3.3.3-r1 iteration #2](#user-content-failure-pr-35903-head-512e17d-3.3.3-r1-2), after the aforementioned patch.

```
emerge =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-512e17d-3.3.3-r1-4" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/4/)__

USE="-* flac" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-512e17d-3.3.3-r1-5" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/5/)__

USE="-* lv2" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

<a id="success-pr-35903-head-512e17d-3.3.3-r1-6" />__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/6/)__

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

### <a id="pr-35903-head-05d838a-3.4.2-r1" />media-sound/audacity-3.4.2-r1

<a id="success-pr-35903-head-05d838a-3.4.2-r1-1" />__[SUCCESS](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r1/1/)__

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

### <a id="pr-35903-head-05d838a-3.4.2-r2" />media-sound/audacity-3.4.2-r2

<a id="success-pr-35903-head-05d838a-3.4.2-r2-3" />__[SUCCESS](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r2/3/)__

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
