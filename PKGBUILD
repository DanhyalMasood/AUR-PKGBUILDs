# Maintainer: Doron Behar <doron.behar@gmail.com>

pkgname=python-vunit_hdl
_name=vunit_hdl
pkgver=4.0.5
pkgrel=1
pkgdesc="Unit Testing Framework for VHDL/SystemVerilog"
arch=('any')
url="https://vunit.github.io/"
license=('MPL')
groups=()
depends=('python')
makedepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=(!emptydirs)
install=
source=("https://files.pythonhosted.org/packages/source/${_name::1}/${_name}/${_name}-${pkgver}.tar.gz")
md5sums=('0747b3435353b16cd1728b3cb36dcaef')

package() {
  cd "$srcdir/$_name-$pkgver"
  python setup.py install --root="$pkgdir/" --optimize=1
}

# vim:set ts=2 sw=2 et:
