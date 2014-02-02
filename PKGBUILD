
pkgname=tache
pkgver=1.0
pkgrel=1
pkgdesc="A simple task manager in command line"
arch=('x86_64')
url="https://www.github.com/bvaudour/tache"
license=('custom')
depends=('java-environment')
source=("https://github.com/bvaudour/tache/raw/master/archives/${pkgname}-${pkgver}.tar.gz")
md5sums=('710c80b4356defa283553fab7c6cc419')

package() {
    cd "$srcdir"
    install -d -m755 "${pkgdir}"/usr/bin/
    install -d -m755 "${pkgdir}"/usr/share/tache/
    install -D -m755 tache/usr/bin/tache "${pkgdir}"/usr/bin/tache
    cp tache/usr/share/tache/* "${pkgdir}"/usr/share/tache/
}

