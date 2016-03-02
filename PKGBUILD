pkgname=caja-term
pkgver=0.1
pkgrel=1
pkgdesc="embedded terminal for Caja, fork of caja-terminal"
arch=('any')
url="https://github.com/mekatronik-achmadi/caja-term"
license=('custom')
depends=('caja' 'vte' 'pygtk' 'python2-caja' 'python2-xdg')
makedepends=
options=('!makeflags')
source=(${pkgname}-master.zip::https://codeload.github.com/mekatronik-achmadi/caja-term/zip/master)
sha256sums=('SKIP')

package() {
	cd "$srcdir"
	unzip -qqo ${pkgname}-master.zip

	install -d $pkgdir/usr/share/
	mv -vf $srcdir/${pkgname}-master/* $pkgdir/usr/share/
}
