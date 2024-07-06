# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <youremail@domain.com>
pkgname=zig
pkgver=0.13.0
pkgrel=1
epoch=
pkgdesc="a general-purpose programming language and toolchain for
    maintaining robust, optimal, and reusable software"
arch=(x86_64)
url=""
license=('MIT')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=("zig=$pkgver")
conflicts=("zig<$pkgver")
replaces=()
backup=()
options=()
install=
changelog=
source=("https://ziglang.org/download/${pkgver}/zig-linux-${arch}-${pkgver}.tar.xz")
noextract=()
sha256sums=(SKIP)
validpgpkeys=()

prepare() {
	cd "zig-linux-${arch}-${pkgver}"

}

build() {
	cd "zig-linux-${arch}-${pkgver}"
}

check() {
	cd "zig-linux-${arch}-${pkgver}"
}

package() {
	cd "zig-linux-${arch}-${pkgver}"
	mkdir -p "$pkgdir/usr/lib"
	cp -r lib "$pkgdir/usr/lib/zig"
	install -Dm755 zig "$pkgdir/usr/bin/zig"



}
