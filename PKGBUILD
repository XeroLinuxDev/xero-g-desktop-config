# Maintainer: DarkXero <info@techxero.com>
pkgname=desktop-config-gnome
_pkgname=xero-g-desktop-config
_destname1="/etc"
pkgver=1.2
pkgrel=1
pkgdesc="Desktop Config for XeroG"
arch=('any')
url="https://github.com/XeroLinuxDev"
license=('GPL3')
makedepends=('git')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${_pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
	rm ${srcdir}/${pkgname}/LICENSE
}
