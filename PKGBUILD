# Maintainer: Jacob Stannix <jakestannix@gmail.com>
pkgname=zig
pkgver=0.13.0
pkgrel=1
pkgdesc="a general-purpose programming language and toolchain for
    maintaining robust, optimal, and reusable software"
arch=(x86_64)
url="ziglang.org"
license=('MIT')
provides=("zig=$pkgver")
conflicts=("zig<$pkgver")
source=("https://ziglang.org/download/${pkgver}/zig-linux-${arch}-${pkgver}.tar.xz")
sha256sums=(d45312e61ebcc48032b77bc4cf7fd6915c11fa16e4aad116b66c9468211230ea)

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
