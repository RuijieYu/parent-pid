#!/usr/bin/env false # PKGBUILD
# vim: syntax=bash

pkgname=parent-pid
pkgver=v0.0.1
pkgrel=1
pkgdesc='Provide a script that shows the parent pid for a given pid'
depends=()
source=(parent)
md5sums=(SKIP)
arch=(any)
license=(MIT)

pkgver() (
    echo v0.0.1
)

package() (
    install -Dm755 "$srcdir/parent" "$pkgdir/usr/bin/parent"
)

