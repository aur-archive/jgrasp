# Maintainer: Your Name <youremail@domain.com>
pkgname=jgrasp
pkgver=2.0.0_14
pkgrel=2
pkgdesc="An Integrated Development Environment with Visualizations for Improving Software Comprehensibility"
arch=('i686' 'x86_64')
url="http://www.jgrasp.org/"
license=('GPL')
groups=('devel')
depends=('java-runtime' 'ld-lsb')
optdepends=('java-environment: needed for developing Java programs')
install='jgrasp.install'
source=('jGRASP.desktop'
	'https://github.com/butangmucat/aur-file-mirrors/raw/master/jgrasp200_14.zip') #Mirrored because it cannot be downloaded without a browser visiting the download page
md5sums=('b2732e31e3f8343b225bd1c7063caafe'
	'65cd43c6406ca1e03cf5e1773d6ac5cf')

package() {
	cd "$srcdir/"
	mkdir -p "$pkgdir/usr/share/applications/"
	mkdir -p "$pkgdir/opt/"
	cp -r jgrasp "$pkgdir/opt/"
	cp ../jGRASP.desktop "$pkgdir/usr/share/applications/"
}
