__THIS REPO IS SUBJECT TO FORCED PUSH__

# media-sound/audacity

## PR 35903 HEAD 512e17d

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

### media-sound/audacity-3.3.3-r1

__[SUCCESS](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/1/)__

USE="-*" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.3.3-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.3.3-r1-*
emerge -k =media-sound/audacity-3.3.3-r1
```

__[FAILURE](results/PR_35903/head_512e17d21024862b7e2f58025fe72354863ee345/media-sound/audacity/audacity-3.3.3-r1/2/)__

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

Resuming from a previous failure, after the aforementioned patch.

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

## PR 35903 HEAD 05d838a

__LXC container__: _Gentoo amd64 (openrc) (20240406_16:07)_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#05d838a](https://github.com/Jamim/gentoo/tree/05d838a28b1c2516741f7ff25b2c4e89984e76e8)  
Head of Gentoo's repo: [gentoo/gentoo#be766b5](https://github.com/gentoo/gentoo/tree/be766b5b349fc88b7c91c35074560d162240c3fd)

### media-sound/audacity-3.4.2-r1

USE="-alsa -audiocom -ffmpeg -flac -id3tag -ladspa -lv2 -mpg123 -ogg -opus -portmixer -sbsms -test -twolame -vamp -vorbis -wavpack" ABI_X86="(64)"

__[SUCCESS](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r1/1/)__

```
emerge =media-sound/audacity-3.4.2-r1
```

__[FAILURE](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r1/2/)__

```
emerge --unmerge media-sound/audacity
emerge --depclean
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```

### media-sound/audacity-3.4.2-r2

USE="-alsa -audiocom -ffmpeg -flac -id3tag -ladspa -lv2 -mpg123 -ogg -opus -portmixer -sbsms -test -twolame -vamp -vorbis -wavpack" ABI_X86="(64)"

__[SUCCESS](results/PR_35903/head_05d838a28b1c2516741f7ff25b2c4e89984e76e8/media-sound/audacity/audacity-3.4.2-r2/3/)__

```
cd /var/db/repos/localrepo/media-sound/audacity
cp audacity-3.4.2-r{1,2}.ebuild
patch -p1 < .../audacity-3.4.2-r2-3.patch
ebuild audacity-3.4.2-r2.ebuild manifest
emerge --unmerge media-sound/audacity
emerge --depclean
emerge -k =media-sound/audacity-3.4.2-r2
```
