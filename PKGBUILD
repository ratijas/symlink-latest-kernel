# Maintainer: ivan a.k.a. ratijas <me@ratijas.tk>
pkgname=symlink-latest-kernel
pkgver=1.0
pkgrel=1
pkgdesc="Symlink latest kernel version in /usr/lib/modules"
arch=('any')
url="https://github.com/ratijas/symlink-latest-kernel"
license=('GPL2')
depends=(linux)
install=
source=(
    symlink-latest-kernel
    symlink-latest-kernel.hook
    )
sha512sums=(
    1a76c37b3a2cc33f893795e501314cbe776e4d2d20c3beca91240909a5e2f03c
    b27b009c4736d632a82238c08c45328882b7966ee4f1e5157e08c128eb4f392f
    )

package() {
    install -Dm 755 "${srcdir}/symlink-latest-kernel"      "${pkgdir}/usr/share/libalpm/scripts/symlink-latest-kernel"
    install -Dm 644 "${srcdir}/symlink-latest-kernel.hook" "${pkgdir}/usr/share/libalpm/hooks/symlink-latest-kernel.hook"
}
