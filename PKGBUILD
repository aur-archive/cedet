# $Id: PKGBUILD 70096 2012-04-29 09:24:02Z spupykin $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>

pkgname=cedet
pkgver=1.1
pkgrel=1
pkgdesc="tools written with the end goal of creating an advanced development environment in Emacs."
arch=(any)
url="http://cedet.sourceforge.net/"
license=('GPL')
depends=(emacs)
install=cedet.install
source=(http://downloads.sourceforge.net/cedet/$pkgname-$pkgver.tar.gz)
md5sums=('a570ed74bfe8b5690e48d01518c2bd29')

build() {
  cd $srcdir/$pkgname-$pkgver
  make
  mkdir -p $pkgdir/usr/share/emacs/site-lisp/cedet
  cp -R $srcdir/$pkgname-$pkgver/* $pkgdir/usr/share/emacs/site-lisp/cedet
}
