# Contributor: Kodai Matsumoto <nobita.0918@gmail.com>

pkgname=arch-pkg-example
pkgver=0.1
pkgrel=1
arch=('x86_64')
pkgdesc="Arch linux package example"
url="https://github.com/0918nobita/arch-pkg-example"
license=('MIT')
makedepends=('ocaml')
build() {
    ocamlopt -o hello main.ml
    rm -f *.cmi *.cmx *.o
}
package() {
    mkdir -p "$pkgdir/usr/bin"
    mv hello "$pkgdir/usr/bin"
}
