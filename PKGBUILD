<<<<<<< HEAD
# Maintainer: Murat Çileli <murat.cileli@gmail.com>
pkgname="adwaita-creamy"
pkgver=1.0
pkgrel=1
=======
# Maintainer: Stoyan Minaev <stoyan.minaev@gmail.com>

pkgbase="pkgbase"
pkgname="loli"
pkgver="0.8"
pkgrel="1"
pkgdesc="Loli is a embedded programming language"
arch=("x86_64")
license=("MIT")
url="http://loli-lang.ml/"
makedepends=("git" "cmake" "make" "gcc")
provides=("loli")

source=("loli-$pkgver::git+https://github.com/loli-foundation/loli.git#tag=$pkgver")
sha256sums=("SKIP")

build() {
    cd "${pkgname}-${pkgver}"
    mkdir -p ./build
    cmake -S ./ -B ./build
    cd ./build && make
}

package() {
    cd "$srcdir/${pkgname}-${pkgver}"
    mkdir -p $pkgdir/usr/{bin,lib}
    install -m 755 ./build/loli $pkgdir/usr/bin/
    install -m 755 ./build/libloli.so $pkgdir/usr/lib/
}
>>>>>>> cba40c42f56ab8e9650a84eb5ca9e1e2ef388d4d
