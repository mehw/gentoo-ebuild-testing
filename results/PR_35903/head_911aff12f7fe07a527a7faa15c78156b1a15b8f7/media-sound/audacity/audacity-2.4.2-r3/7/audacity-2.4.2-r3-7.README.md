`media-sound/audacity-2.4.2-r3[doc]: PR 35903 HEAD 911aff1 SUCCESS`

Use `media-libs/libsndfile[minimal]` to not install dependencies
beyond `media-sound/audacity` strict requirements.

`media-libs/libsndfile-1.2.2-r2[!minimal]` would install:
- `media-libs/flac`
- `media-libs/libogg`
- `media-libs/libvorbis`
- `media-libs/opus`
- `media-sound/lame`
- `media-sound/mpg123-base`

---

LXC container: Gentoo amd64 openrc 20240408_16:07

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#911aff1](https://github.com/Jamim/gentoo/tree/911aff12f7fe07a527a7faa15c78156b1a15b8f7)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)
