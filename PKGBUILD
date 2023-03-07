_mode=cross
_nodeps=true
pkgname=device-sm8150-xiaomi-nabu
pkgver=0.3
pkgrel=1
_arches=specific
arch=(aarch64)
license=(MIT)
depends=(
    linux-sm8150-nabu
    firmware-sm8150-xiaomi-nabu
    pd-mapper-git
    tqftpserv-git
    boot-android-common
)
install=sm8150-nabu.install
source=(
    machine-info
    deviceinfo
    xiaomi-nabu.conf
)
sha256sums=(
    7729d6a89258b470cadd48cfbc704bab7791501c53f45f50737dea6b441a3171
    SKIP
    SKIP
)

package() {
    install -Dm644 "$srcdir"/machine-info "$pkgdir"/etc/machine-info
    install -Dm644 "$srcdir"/deviceinfo "$pkgdir"/etc/kupfer/deviceinfo
}
