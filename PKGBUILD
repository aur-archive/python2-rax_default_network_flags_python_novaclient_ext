# Maintainer: Troy Cox <troy.cox@rackspace.com>

pkgname=python2-rax_default_network_flags_python_novaclient_ext
pkgver=0.1.3
pkgrel=0
pkgdesc="Novaclient Extension for Instance Default Network Flags"
arch=('i686' 'x86_64')
url="http://pypi.python.org/pypi/rax-default-network-flags-python-novaclient-ext/0.1"
license=('GPL')
depends=('python2' 'python2-novaclient' 'python2-httplib2' 'python2-prettytable' 'python-simplejson' 'python2-iso8601')
makedepends=('python2')
provides=("python2-rax-default-network-flags-python-novaclient-ext=$pkgver")
source=(http://pypi.python.org/packages/source/r/rax_default_network_flags_python_novaclient_ext/rax_default_network_flags_python_novaclient_ext-${pkgver}.tar.gz)
md5sums=('3afdb8056570f5d4d64cbd70bb505914')

build() {
  cd "$srcdir/rax_default_network_flags_python_novaclient_ext-0.1.3"
  python2 setup.py build || return 1
  python2 setup.py install --root=${pkgdir} || return 1
}
