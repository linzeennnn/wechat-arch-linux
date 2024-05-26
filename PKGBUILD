# Maintainer: linzeen
# Contributor: linzeen
pkgname=wechat-archlinux
makedepends=('dpkg')
pkgver=1.0.0.238
pkgrel=1
pkgdesc="Wechat for Arch Linux"
source=("https://archive2.kylinos.cn/deb/kylin/production/PART-V10-SP1/custom/partner/V10-SP1/pool/all/wechat-beta_1.0.0.238_amd64.deb")
arch=('x86_64')
url="weixin.qq.com"
license=('PGP')
depends=('alsa-lib' 'at-spi2-core' 'cairo' 'dbus' 'expat' 'fontconfig' 'glib2' 'libdrm' 'libx11' 'libxcb' 'libxcomposite' 'libxdamage' 'libxext' 'libxfixes' 'libxrandr' 'libxrender' 'mesa' 'nspr' 'nss' 'pango' 'xcb-util-image' 'xcb-util-keysyms' 'xcb-util-renderutil' 'xcb-util-wm' 'zlib' 'lsb-release')
provides=('wechat')
options=('!strip' '!emptydirs')
install=${pkgname}.install
package(){
dpkg -X wechat-beta_1.0.0.238_amd64.deb "${srcdir}/"
mv "${srcdir}/opt/wechat-beta" "${srcdir}/opt/wechat}"
cp -r "${srcdir}/opt" "${pkgdir}/"
cp -r "${srcdir}/usr" "${pkgdir}/"
cp -r "${srcdir}/etc" "${pkgdir}/"
}
