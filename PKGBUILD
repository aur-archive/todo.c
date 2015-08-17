# Maintainer: Rafael Beraldo <rafaelluisberaldo@gmail.com>

pkgname=todo.c
pkgver=0.2.1
pkgrel=1
pkgdesc="Command line lightweight todo tool with readable storage, written in C."
arch=('i686' 'x86_64')
url="https://github.com/hit9/todo.c"
license=('BSD')
makedepends=('git')
source=($pkgname::git+git://github.com/hit9/todo.c.git)
md5sums=('SKIP')

build() {
  cd "$srcdir/$pkgname"
  make compile
}

package() {
  cd "$srcdir/$pkgname/src/"
  install -v -D -m 0755 todo "${pkgdir}/usr/bin/todo"
}

# vim:set ts=2 sw=2 et:
