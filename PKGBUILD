pkgbase='python-discord-py-interactions'
pkgname=('python-discord-py-interactions')
_module='discord-py-interactions'
pkgver='5.10.0'
pkgrel=1
pkgdesc="Easy, simple, scalable and modular: a Python API wrapper for interactions."
url="https://github.com/interactions-py/interactions.py"
depends=('python')
makedepends=('python-setuptools')
license=('MIT')
arch=('any')
source=("https://files.pythonhosted.org/packages/d2/00/5c3a37ff6b562df6eb3993518c00510ae5154f1875984f62efac44268c24/discord-py-interactions-5.10.0.tar.gz")
sha256sums=('6c7b9e168f1e9ea07481ad1ded5cdd7ecd3f61921ed59d21f4e21d013e4c0aae')

build() {
    cd "${srcdir}/${_module}-${pkgver}"
    python setup.py build
}

package() {
    depends+=()
    cd "${srcdir}/${_module}-${pkgver}"
    python setup.py install --root="${pkgdir}" --optimize=1 --skip-build
}
