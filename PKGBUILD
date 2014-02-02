
pkgname=tache
pkgver=1.0
pkgrel=1
pkgdesc="A simple task manager in command line"
arch=('x86_64')
url="https://www.github.com/bvaudour/tache"
license=('custom')
depends=('java-environment')
source=("https://github.com/bvaudour/tache/releases/download/v${pkgver}/${pkgname}-${arch}.tar.gz"
        "tache")
md5sums=('cf5d913916fdecc726863b3156d03b47'
         '0a48b2a15f7a85b8ea826f38780b8ee3')

package() {
    install -d -m755 "${pkgdir}"/usr/bin/
    install -D -m755 tache "${pkgdir}"/usr/bin/tache
    cd "$srcdir"
    install -d -m755 "${pkgdir}"/usr/share/tache/
    cp tache.jar "${pkgdir}"/usr/share/tache/
}

