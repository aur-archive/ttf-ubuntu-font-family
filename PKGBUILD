# Maintainer: Massimiliano Torromeo <massimiliano.torromeo@gmail.com>

pkgname=ttf-ubuntu-font-family
pkgver=0.80
pkgrel=1
pkgdesc="Ubuntu font family"
arch=('any')
url="http://font.ubuntu.com/"
license=("custom:Ubuntu Font Licence 1.0")
depends=('fontconfig')
install=ttf-ubuntu-font-family.install

_pkgname=ubuntu-font-family

source=(http://font.ubuntu.com/download/${_pkgname}-${pkgver}.zip)

build() {
	cd "${srcdir}/${_pkgname}-${pkgver}"
	install -m755 -d "${pkgdir}/usr/share/fonts/TTF"
	install -m644 ./*.ttf "${pkgdir}/usr/share/fonts/TTF/"
	install -D -m644 LICENCE.txt "${pkgdir}/usr/share/licenses/${pkgname}/LICENCE"
}

md5sums=('a1fc70f5a5b1d096ab8310886cddaa1c')
