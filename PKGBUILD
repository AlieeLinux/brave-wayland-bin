# Maintainer: Ali Ali <AliAliee@localhost.com>

pkgname=brave-wayland
pkgver=1
pkgrel=1
pkgdesc="Mini packge that adds wayland support on brave-browser"
arch=('x86_64')
url="https://brave.com/"
license=('MIT')
optdepends=('brave-bin: Browser that block ads by default')
source=("brave-browser-wayland.desktop")
sha256sums=('b925cc2ac25cb038b596134d7001f7ebb1ce0c11c82a9e036f3534711d5ab323')

build() {
    mkdir -p "$srcdir/usr/share/applications"
    cp ./brave-browser-wayland.desktop "$srcdir/usr/share/applications"
}

package() {
    cp -rvf "usr" "$pkgdir/"
}

clean() {
    rm -rvf "$srcdir"
}
