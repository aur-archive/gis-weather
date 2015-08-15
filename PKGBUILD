# Maintainer: Pokhodyun Alexander (Karbunkul) <karbunkul@yourtask.ru>
pkgname=gis-weather
pkgver=0.7.5
pkgrel=1
pkgdesc="Customizable weather widget"
arch=('i686' 'x86_64')
url="http://sourceforge.net/projects/gis-weather"
license=('GPLv3')
depends=('gtk3' 'python' 'python-gobject')
optdepends=('librsvg')

source=(${url}/files/gis-weather/${pkgver}/gis-weather_${pkgver}_all.deb/download)
md5sums=('763631f595717157b0d9b5ef3c8d88a2')

package() {
  cd "$srcdir"
  tar -xf data.tar.xz -C "${pkgdir}"
  echo "aur" > "${pkgdir}/usr/share/${pkgname}/package"
  chmod -R 777 "${pkgdir}"/usr/share/${pkgname}
  mkdir -p $pkgdir/usr/bin
}
