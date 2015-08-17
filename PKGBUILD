# Maintainer: Keith Hughitt <khughitt@umd.edu>
pkgname=python-glymur
pkgver=0.5.12
pkgrel=1
pkgdesc="Tools for accessing JPEG2000 files"
url="https://github.com/quintusdias/glymur"
depends=('python' 'openjpeg')
makedepends=('python' )
license=('MIT')
arch=('any')
source=('https://pypi.python.org/packages/source/G/Glymur/Glymur-0.5.6.tar.gz')
md5sums=('772e4a37600e4c9603765d2762a9f7e8')

build() {
    cd $srcdir/Glymur-0.5.6
    python setup.py build
}

package() {
    cd $srcdir/Glymur-0.5.6
    python setup.py install --root="$pkgdir" --optimize=1
}
