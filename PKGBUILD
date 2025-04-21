pkgname=nyaafet
pkgver=1.0.0
pkgrel=1
pkgdesc="CLI tool to quickly torrent from nyaa using fzf"
arch=('x86_64')
url="https://github.com/PSxUchiha/nyaafet"
license=('GPL3') 
depends=('bash' 'curl' 'grep' 'fzf')
provides=('nyaafet')
source_x86_64=("https://github.com/PSxUchiha/nyaafet/releases/download/${pkgver}/nyaafet-${pkgver}")
noextract=("nyaafet-${pkgver}")
sha256sums_x86_64=('d9de547694afd74328866b831357da53e116afb6e6e76f438decc1a543315c87')
package() {
  install -Dm755 "nyaafet-${pkgver}" "${pkgdir}/usr/bin/nyaafet"
}

