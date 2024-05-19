# Maintainer: Caleb Maclennan <caleb@alerque.com>
# Maintainer: Bruno Pagani <archange@archlinux.org>

pkgver=30
pkgrel=2
epoch=1
pkgname=electron-xdg
pkgdesc='Meta package providing the latest available stable Electron build - patched to support the xdg basedir spec'
arch=(any)
url='https://electronjs.org'
license=(MIT)
depends=("electron$pkgver-xdg")
conflicts=("electron")
provides=("electron")

package() {
	mkdir -p "$pkgdir/usr/bin" "$pkgdir/usr/lib"
	ln -sf "${depends[0]}" "$pkgdir/usr/bin/$pkgname"
	ln -sf "${depends[0]}" "$pkgdir/usr/lib/$pkgname"
}
