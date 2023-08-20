pkgname=bbgl
pkgver=2.4.6
pkgrel=1
arch=('x86_64')
source=('https://www.jbysoft.com/r/cms/www/default/download_zs/bb_amd64.deb' 'bbgl.desktop')

sha512sums=("SKIP" "SKIP")
package(){
	echo "Decompressing deb package..."
	bsdtar -xf ${srcdir}/data.tar.xz -C ${pkgdir}
	echo "Deb package successfully decompressed!"
	rm -r ${pkgdir}/usr/share/lintian
	echo "Successfully removed lintian check results!"
	install -Dm 644 ${srcdir}/bbgl.desktop ${pkgdir}/usr/share/applications/

}
