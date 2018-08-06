# Maintainer: liberodark

pkgname=ifl
pkgver=3.21
pkgrel=1
pkgdesc="TeraByte Image for Linux"
arch=('x86_64')
url="https://www.terabyteunlimited.com/image-for-linux.htm"
license=('Custom')
depends=('xdg-utils' 'gksu-polkit' 'sshfs' 'lib32-libxft' 'lib32-libpng12' 'lib32-libxinerama')
source_x86_64=("ifl.tar.gz")
source=($pkgname.desktop
        $pkgname.png)
sha512sums=('dd4e4b7052a02ea4d9dc0390cc6413d81017ed6635df49a6af7fde2a503711cda29da1e2b5eb410442d6b03aaa1f60c3315d636c86c9be78f7909d5fc0fd09fd'
         'c9ff35d9dcd25020d41a5f4cd06efc830947fe617facd0ef6895bee01f8f00f6cee7842dd29c304bdcc1f2f1e76b880ea356e5bcc8ee6a5eccaece5bca70ad4e')
sha512sums_x86_64=('902dd73516e9e6191b2549f49643f1b636f01b938f230c3d8f756105dc7c71537ca42bca5f937ca236506ead77dfc91c83a1dcaf779639f33ef746ce9618bbb0')
        
package() {
  cd $srcdir
  tar xvf ifl.tar.gz
  mkdir -p "$pkgdir/opt/ifl"
  cp -r "ifl/." "$pkgdir/opt/ifl"
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}
