pkgname=tache
pkgver=1.0
pkgrel=1
pkgdesc="A simple task manager in command line"
arch=('x86_64')
url="https://www.github.com/bvaudour/tache"
license=('custom')
depends=('java-environment')

build() {
	cd ${srcdir}
	git clone "${url}.git"
}

package() {
	cd "${srcdir}/${pkgname}/archives/"
	bsdtar -xf "${pkgname}-${pkgver}.tar.gz" -C "${pkgdir}/"
}
