#!/usr/bin/env false # PKGBUILD
# vim: syntax=bash

pkgname=parent-pid-git
_pkgname="${pkgname%-git}"

pkgver=rev2.144069a
pkgrel=1
pkgdesc='A simple program that shows the parent pid for a given pid'

depends=()
makedepends=('git')
conflicts=("$_pkgname")
arch=(any)

license=(MIT)

url="https://github.com/RuijieYu/$_pkgname"
source=("$_pkgname::git+$url.git#branch=master")
md5sums=(SKIP)

pkgver() (
    cd "$srcdir/$_pkgname"
    printf rev%d.%s "$(git rev-list --count @)" "$(git rev-parse --short @)"
)

package() (
    install -Dm755 "$srcdir/$_pkgname/parent" "$pkgdir/usr/bin/parent"
)

