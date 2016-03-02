pkgname=caja-term
pkgver=0.1
pkgrel=1
pkgdesc="embedded terminal for Caja, fork of caja-terminal"
arch=('any')
url=
license=('custom')
depends=('caja' 'vte' 'pygtk' 'python2-caja' 'python2-xdg')
makedepends=
options=('!makeflags')
source=(${pkgname}-master.zip)
sha256sums=('SKIP')

package() {
	cd "$srcdir"
	unzip -qqo ${source}

	install -d $pkgdir/usr/share/
	mv -vf $srcdir/${pkgname}-master/* $pkgdir/usr/share/
}
