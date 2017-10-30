# Maintainer: Simone Sclavi 'Ito' <darkhado@gmail.com>
# Contributor: Changaco <changaco@changaco.net>
# Contibutor : Jean Prat (see github https://github.com/saez0pub/mbrola-archlinux)


pkgname=mbrola
pkgver=3.02b
_mypkgv=${pkgver//./}
pkgrel=4
pkgdesc="A phoneme-to-audio converter used by many TTS (Text-to-speech) programs."
arch=('armv7h')
url="http://tcts.fpms.ac.be/synthesis/mbrola.html"
license=('custom:Mbrola')
source=(http://tcts.fpms.ac.be/synthesis/mbrola/bin/raspberri_pi/mbrola.tgz
        LICENSE)
md5sums=('f49d8607929fbe9c3931e7a18fa10368'
         '3ec25133449591ade620fa694e1e9546')
[ $CARCH = "armv7h" ] &&  depends=('glibc')
package() {
  install -Dm755 mbrola $pkgdir/usr/bin/$pkgname  
  install -Dm644 LICENSE ${pkgdir}/usr/share/licenses/${pkgname}/LICENSE 
}
