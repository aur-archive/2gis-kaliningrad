pkgname=2gis-kaliningrad
pkgver=29
pkgrel=1
pkgdesc="Map of Kaliningrad for 2GIS, July 2013"
arch=('i686' 'x86_64')
url="http://kaliningrad.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Kaliningrad-29.orig.zip")
md5sums=('0c5ba61cf58709004c98085d531669f3')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Kaliningrad.dgdat" "${pkgdir}/opt/2gis/kaliningrad.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Kaliningrad.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/kaliningrad.dglf" || return 1
}
