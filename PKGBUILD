# Maintainer: MartorSkull <livemartor@gmail.com>
pkgname=plutus-tools
pkgver=0.1.1
pkgrel=1
pkgdesc="Utilities for cardano smart contract development"
provides=('plutus-tools')
arch=('x86_64')
license=('MIT')
source=(
    "plutus"
    "plutus.sh"
)
sha256sums=(
    "f701ef374a1ecee642e2da76af16dfce3eb86191b8c6bbe470bf6a920eebf09f"
    "cb799ace7f4c3e1272521cf11445b3c378e3b72e99fcdcf71d8d24f32864565a"
)
depends=(git nix)
package() {
    install -Dm755 "${srcdir}/plutus" "${pkgdir}/usr/bin/plutus"
    install -Dm644 "${srcdir}/plutus.sh" "${pkgdir}/etc/profile.d/plutus.sh"
}
