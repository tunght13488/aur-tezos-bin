# Maintainer: Vincent Bernardoff <vb@luminar.eu.org>

pkgname=tezos-bin
pkgver=11.0_1
pkgrel=1
pkgdesc='Tezos static binaries by Serokell'
arch=('x86_64')
url='https://github.com/serokell/tezos-packaging'
license=('MIT')
provides=('tezos')
conflicts=('tezos')
options=(!strip)
depends=()
source=("https://github.com/serokell/tezos-packaging/releases/download/v${pkgver//_/-}/binaries-${pkgver//_/-}.tar.gz"
        "https://github.com/serokell/tezos-packaging/releases/download/v${pkgver//_/-}/binaries-${pkgver//_/-}.tar.gz.asc")
sha512sums=('0d0b4765456968e71c3bf6fe824c717b4031495822daf2794bf3ca95367ae1a6cf0c22462030ad2f26e9d499201b5f7026066bc960a3eaad1b4b253d54fdc36e'
            'SKIP')
validpgpkeys=("7EAF9B150ACE940CF8C008A0BF847A85AC7BF43E")

package() {
  cd ${srcdir}
  dst="${pkgdir}/usr/bin"
  mkdir -p ${dst}
  install tezos-* ${dst}
}
