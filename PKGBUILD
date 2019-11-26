# Maintainer: Samuel Williams <samuel@oriontransfer.net>

pkgname=github-actions
pkgver=2.161.0
pkgrel=1
pkgdesc='GitHub Actions self-hosted runner tools.'
arch=('x86_64')
url='https://help.github.com/en/actions'
license=('custom')

provides=('github-actions')
conflicts=('github-actions')

source=(
	https://githubassets.azureedge.net/runners/$pkgver/actions-runner-linux-x64-$pkgver.tar.gz
)

sha512sums=('711cdb99e6dc34e6cc843ef31befd2db49bfe0463f3da9550663ced9febb362cdf23d4976ce78455edad72d00dd0713114e13c46a5461c454a5a9fe5738b8639')

package() {
  mkdir -p "$pkgdir/opt/$provides" 
  cp -r "$srcdir/." "$pkgdir/opt/$provides"
}
