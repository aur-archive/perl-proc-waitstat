# Contributor: Andreas Wagner < Andreas dot Wagner at em dot uni-frankfurt dot de >

pkgname=perl-proc-waitstat
pkgver=1.00
pkgrel=5
pkgdesc="Functions for interpreting and acting on wait() status values"
arch=(any)
url="http://www.argon.org/~roderick/"
license=('PerlArtistic')
depends=('perl-ipc-signal')
source=(http://www.argon.org/~roderick/Proc-WaitStat-$pkgver.tar.gz)
md5sums=('b911bd579b6b142391b21de1efa30c95')

build() {
  cd "${srcdir}/Proc-WaitStat-$pkgver"
  perl Makefile.PL
}

package() {
  cd "${srcdir}/Proc-WaitStat-$pkgver"
  make install DESTDIR=${pkgdir}
}
