
# Maintainer: Juan Toca <elan17.programacion@gmail.com>
pkgname=snakes-git
pkgver=1.0
pkgrel=1
pkgdesc="Snake-based ZPG game"
arch=('x86_64')
url="https://github.com/elan17/snakes-terminalsaver"
license=('GPL')
groups=()
depends=()
makedepends=('git' 'python') 
provides=("${pkgname%-VCS}")
conflicts=("${pkgname%-VCS}")
replaces=()
backup=()
options=(!emptydirs)
install=
source=('snakes-git::git+https://github.com/elan17/snakes-terminalsaver#branch=master')
noextract=()
md5sums=('SKIP')

pkgver() {
   date +%Y%m%d
}

package() {
	cd "$srcdir/$pkgname"
  	install -Dm 755 snakes.py "${pkgdir}/usr/bin/snakes"
  	install -Dm 644 LICENSE "${pkgdir}/usr/share/doc/${pkgname}/LICENSE"
}

