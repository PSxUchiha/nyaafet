pkgname=nyaafet
pkgver=1.0.1
pkgrel=1
pkgdesc="CLI tool to quickly torrent from nyaa using fzf"
arch=('x86_64')
url="https://github.com/PSxUchiha/nyaafet"
license=('GPL3') 
depends=('bash' 'curl' 'grep' 'fzf')
provides=('nyaafet')
source_x86_64=("https://github.com/PSxUchiha/nyaafet/releases/download/${pkgver}/nyaafet-${pkgver}")
noextract=("nyaafet-${pkgver}")
sha256sums_x86_64=('8a332ed344e7c8661dcf5544ef27c8aa96cec0cea1829f5dc3732b70d17cfc7a')
package() {
  install -Dm755 "nyaafet-${pkgver}" "${pkgdir}/usr/bin/nyaafet"
}

