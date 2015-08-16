# Maintainer: Bastien Dejean <baskerville at lavabit.com>

pkgname=libuninameslist
pkgver=20091231
pkgrel=2
pkgdesc='Unicode annotations helper'
arch=('i686' 'x86_64')
url='http://libuninameslist.sourceforge.net/'
license=('BSD')
provides=('libuninameslist')
conflicts=('libuninameslist')
source=("http://downloads.sourceforge.net/project/libuninameslist/libuninameslist%20sources/Unicode_5.2-$pkgver/libuninameslist-$pkgver.tar.bz2")
md5sums=('14f47d50fb0e05c5029298847437feab')

build() {
    cd "$srcdir/$pkgname"
    ./configure --prefix=/usr
    make
}

package() {
    cd "$srcdir/$pkgname"
    make DESTDIR="$pkgdir" install
}
