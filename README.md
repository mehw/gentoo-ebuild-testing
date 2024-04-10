__THIS REPO IS SUBJECT TO FORCED PUSH__

# media-sound/audacity

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
