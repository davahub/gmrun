
pkgname=gmrun
pkgver=1.4w
pkgrel=1
pkgdesc="A simple program which provides a run program window"
arch=('x86_64')
url="https://github.com/wdlkmpx/gmrun"
license=('GPL')
depends=('gtk3' 'popt')
build() {
  cd "$HOME/workspace/gmrun"
	./configure --prefix=/usr --sysconfdir=/etc
	make
}

package() {
  cd "$HOME/workspace/gmrun"
	make DESTDIR="${pkgdir}" install
}
