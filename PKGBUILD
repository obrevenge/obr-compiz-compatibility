# Maintainer: Jody James <ajjamesobr@gmail.com>

pkgname=obr-compiz-compatibility
pkgver=1.01
pkgrel=1
pkgdesc="Compiz Compatibility Package for OBRevenge"
arch=('any')
license=('GPL')
depends=('compiz')
source=("git+https://github.com/obrevenge/obr-compiz-compatibility.git")
md5sums=('SKIP')


package() {
    
    mkdir -p "${pkgdir}/etc/skel/.config"
    cp -rf "${scrdir}obr-compiz-compatibility/compiz" "${pkgdir}/etc/skel/.config"
    cp -rf "${scrdir}obr-compiz-compatibility/compiz-1" "${pkgdir}/etc/skel/.config"
    mkdir -p "${pkgdir}/usr/share/xsessions"
    cp "${scrdir}obr-compiz-compatibility/compiz.desktop" "$/usr/share/xsessions"
    mkdir -p "${pkgdir}/usr/bin"
    cp "${scrdir}obr-compiz-compatibility/compiz-session-start.sh" "${pkgdir}/usr/bin"
    cp "${scrdir}obr-compiz-compatibility/compiz-autostart" "${pkgdir}/usr/bin"
    

}

# -*- mode: bash;-*-

