
pkgname=tache
pkgver=1.1
pkgrel=1
pkgdesc="A simple task manager in command line"
arch=('x86_64')
url="https://www.github.com/bvaudour/tache"
license=('custom')
depends=('java-environment')
source=("https://github.com/bvaudour/tache/releases/download/v${pkgver}/${pkgname}-${arch}.tar.gz"
        "tache")
md5sums=('ffe174bd2ea3e9ca7b4f8afe70a7bb29'
         '0a48b2a15f7a85b8ea826f38780b8ee3')

package() {
    install -d -m755 "${pkgdir}"/usr/bin/
    install -D -m755 tache "${pkgdir}"/usr/bin/tache
    cd "$srcdir"
    install -d -m755 "${pkgdir}"/usr/share/tache/
    cp tache.jar "${pkgdir}"/usr/share/tache/
    install -d -m755 "${pkgdir}"/usr/share/man/man1/
    cp tache.1.gz "${pkgdir}"/usr/share/man/man1/
}

