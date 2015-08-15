# Maintainer: Jakub Klinkovský <kuba.klinkovsky@gmail.com>

pkgname=eclipse-qt-eclipse-integration-bin
pkgver=1.6.1
pkgrel=4
pkgdesc="official binaries of the Qt Eclipse plugin"
arch=("i686" "x86_64")
url="http://qt.nokia.com/developer/eclipse-integration"
license=("LGPL")
depends=("qt4>=4.6" "eclipse>=3.3.2" "eclipse-cdt>=4.0")
conflicts=("eclipse-qt-eclipse-integration")
install=$pkgname.install

[ "$CARCH" = "i686" ] && {
    md5sums=("3bf27fca4dd9051071f4bbf8ff761655")
    _arch="x86"
}
[ "$CARCH" = "x86_64" ] && {
    md5sums=("3b5ad955dd84608de07331509b4ddffb")
    _arch="x86_64"
}
source=("http://get.qt.nokia.com/qteclipse/qt-eclipse-integration-linux.${_arch}-${pkgver}.tar.gz")

package() {
    install -dm755 "$pkgdir/usr/share"
    cp -rp "$srcdir/eclipse" "$pkgdir/usr/share/"
}
