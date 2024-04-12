# media-sound/audacity

## PR 35903 HEAD 05d838a

__LXC container__: _Gentoo amd64 (openrc) (20240406_16:07)_

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#05d838a](https://github.com/Jamim/gentoo/tree/05d838a28b1c2516741f7ff25b2c4e89984e76e8)  
Head of Gentoo's repo: [gentoo/gentoo#be766b5](https://github.com/gentoo/gentoo/tree/be766b5b349fc88b7c91c35074560d162240c3fd)

### media-sound/audacity-3.4.2-r1

__FAILURE__

USE="-*" ABI_X86="(64)"

```
emerge --unmerge media-sound/audacity
emerge --depclean
nano /var/cache/binpkgs/Packages # remove audacity-3.4.2-r1 entries
rm /var/cache/binpkgs/media-sound/audacity/audacity-3.4.2-r1-*
emerge -k =media-sound/audacity-3.4.2-r1
```
