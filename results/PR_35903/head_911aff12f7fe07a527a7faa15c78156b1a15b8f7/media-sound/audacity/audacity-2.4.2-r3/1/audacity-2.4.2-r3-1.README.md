`media-sound/audacity-2.4.2-r3[-*]: PR 35903 HEAD 911aff1 FAILURE`

Undefined references about `libflac`, required by Audacity's ondemand
(aka OD) file handling, even when `libflac` support had been disabled
via configure.

Triggers: [bug#741969](https://bugs.gentoo.org/741969)  
Triggers: [bug#884747](https://bugs.gentoo.org/884747)

Fixed in [`media-sound/audacity-2.4.2-r3[-*]: PR 35903 HEAD 911aff1 SUCCESS (patch)`](https://github.com/mehw/gentoo-ebuild-testing/tree/media-sound/audacity#user-content-success-pr-35903-head-911aff1-2.4.2-r3-2)
via suggested patch.

---

LXC container: Gentoo amd64 openrc 20240408_16:07

Testing PR: [gentoo/gentoo#35903](https://github.com/gentoo/gentoo/pull/35903)  
Head of PR: [Jamim/gentoo#911aff1](https://github.com/Jamim/gentoo/tree/911aff12f7fe07a527a7faa15c78156b1a15b8f7)  
Head of Gentoo's repo: [gentoo/gentoo#9428b7b](https://github.com/gentoo/gentoo/tree/9428b7b54576cfaa84da562e1148a804acd6cc30)
