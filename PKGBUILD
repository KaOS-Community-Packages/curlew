pkgname=curlew
pkgver=0.2.2
pkgrel=1
pkgdesc='Easy to use, Free and Open-Source Multimedia converter for Linux in Python'
arch=('x86_64')
license=('Waqf GPL')
url="http://sourceforge.net/projects/curlew/"
depends=('python3' 'ffmpeg' 'python3-gobject3' 'hicolor-icon-theme' 'gobject-introspection' 'xdg-utils' 'pyxdg' 'dbus-python3' 'mediainfo')
makedepends=('intltool' 'librsvg')
optdepends=('curl: Aurploader support')
source=("http://downloads.sourceforge.net/project/${pkgname}/${pkgname}-${pkgver}/${pkgname}-${pkgver}.tar.gz")
sha256sums=('b2432c97997655543ebd759adfebb37594d270bad980e02db48368886f45e60f')
install="${pkgname}.install"

package() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    python3 setup.py install --prefix=/usr --root="$pkgdir"/ --optimize=1
}
