# Maintainer: MartorSkull <livemartor@gmail.com>
pkgname=plutus-tools
pkgver=0.1.0
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
    "87ce3194cb56e6ecc8c0e0493b2ed4015466c47da38dc5758e84bcb7a6a7f54e"
    "cb799ace7f4c3e1272521cf11445b3c378e3b72e99fcdcf71d8d24f32864565a"
)
depends=(git nix)
package() {
    install -Dm755 "${srcdir}/plutus" "${pkgdir}/usr/bin/plutus"
    install -Dm644 "${srcdir}/plutus.sh" "${pkgdir}/etc/profile.d/plutus.sh"
}
