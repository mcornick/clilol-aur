# This file was generated by GoReleaser. DO NOT EDIT.
# Maintainer: Mark Cornick <mcornick@mcornick.com>

pkgname='clilol-bin'
pkgver=0.9.1
pkgrel=1
pkgdesc='A CLI for omg.lol'
url='https://mcornick.com/clilol/'
arch=('aarch64' 'armv6h' 'i686' 'x86_64')
license=('MPL-2.0')
provides=('clilol')
conflicts=('clilol')

source_aarch64=("${pkgname}_${pkgver}_aarch64.tar.gz::https://github.com/mcornick/clilol/releases/download/v0.9.1/clilol_0.9.1_linux_arm64.tar.gz")
sha256sums_aarch64=('2d7d25c5d57d10ff9bd710ae31417e9d8a5c67c70cfc8c7336d097f57489a9a5')

source_armv6h=("${pkgname}_${pkgver}_armv6h.tar.gz::https://github.com/mcornick/clilol/releases/download/v0.9.1/clilol_0.9.1_linux_armv6.tar.gz")
sha256sums_armv6h=('1d854c6688730804083386296bfb77332e74721376d6c48da5b496afb1130e7a')

source_i686=("${pkgname}_${pkgver}_i686.tar.gz::https://github.com/mcornick/clilol/releases/download/v0.9.1/clilol_0.9.1_linux_386.tar.gz")
sha256sums_i686=('109ed48b9043120b56ee69c48a636843be7baf0516d0fdc17647051c2bb9a3c4')

source_x86_64=("${pkgname}_${pkgver}_x86_64.tar.gz::https://github.com/mcornick/clilol/releases/download/v0.9.1/clilol_0.9.1_linux_amd64.tar.gz")
sha256sums_x86_64=('0eeb59bd0b9c12e4092be25a6576a8620ff8f32b099d8d09f9c1a54f2625ecf6')

package() {
  install -Dm755 "./clilol" "${pkgdir}/usr/bin/clilol"
  install -Dm644 "./LICENSE" "${pkgdir}/usr/share/licenses/clilol/LICENSE"
  mkdir -p "${pkgdir}/usr/share/bash-completion/completions/"
  mkdir -p "${pkgdir}/usr/share/zsh/site-functions/"
  mkdir -p "${pkgdir}/usr/share/fish/vendor_completions.d/"
  install -Dm644 "./completions/clilol.bash" "${pkgdir}/usr/share/bash-completion/completions/clilol"
  install -Dm644 "./completions/clilol.zsh" "${pkgdir}/usr/share/zsh/site-functions/_clilol"
  install -Dm644 "./completions/clilol.fish" "${pkgdir}/usr/share/fish/vendor_completions.d/clilol.fish"
  install -Dm644 "./manpages/*.1" "${pkgdir}/usr/share/man/man1/*.1"
}
