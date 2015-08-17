# Maintainer: Sebastien Luttringer <seblu+arch@seblu.net
# Contributor: Andreas Hauser <andy-aur@splashground.de>
pkgname=nload
pkgver=0.7.3
pkgrel=1
pkgdesc='Console application which monitors network traffic and bandwidth usage in real time'
url='http://www.roland-riegel.de/nload'
license=('GPL2')
depends=('ncurses')
arch=('i686' 'x86_64')
source=("$url/$pkgname-$pkgver.tar.gz")
md5sums=('9b97c37fe1474f1da42f265fead24081')

build() {
  cd $pkgname-$pkgver
  ./configure --prefix=/usr
  make
}

package() {
  cd $pkgname-$pkgver
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 ft=sh et:
