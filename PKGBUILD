# Maintainer: Košava <kosava@archlinux.us>
pkgname=yarock-new
pkgver=0.0.56
pkgrel=1
pkgdesc="Yarock is Qt4 Modern Music Player with collection browser based on cover art."
arch=('i686' 'x86_64')
url="http://qt-apps.org/content/show.php?content=129372"
license=('GPL3')
depends=('qt' 'taglib' 'phonon')
makedepends=('boost')
conflicts=('yarock')
source=(http://launchpad.net/yarock/trunk/0.0.56/+download/Yarock_0.0.56_source.tar.gz yarock.desktop)

build() {
   cd $srcdir/Yarock_0.0.56_source
   qmake PREFIX="/usr/"
   make INSTALL_ROOT=$pkgdir install
ln -s $pkgdir/usr/bin/YaRock $pkgdir/usr/bin/yarock

}
md5sums=('821288c8ed0a2bf4ffe90eba9ab13b08'
         '421d8a602ab1674568e5f553c6fc2694')
