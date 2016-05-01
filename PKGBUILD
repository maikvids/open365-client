pkgname=open365-client
pkgver=1.0.0
pkgrel=1
description="An open source Office365 alternative that allows edit or create documents online"
category=Office
screenshot=http://i.imgur.com/16YkEa1.png?1
arch=('x86_64')
url="https://open365.io"
license=('unknow')
source=("https://s3-eu-west-1.amazonaws.com/open365.io/downloads/open365-client-1.0.0.112428-17.deb")
depends=('python2-simplejson' 'libevent' 'qt' 'glib2' )
md5sums=('120c3764f514c983657004f8f0153cf5')
package() {
 tar -xf data.tar.gz -C $pkgdir
 echo -en "#!/bin/bash\nexec /opt/open365/bin/open365-client"  > $pkgdir/usr/bin/$pkgname
 chmod +x  $pkgdir/usr/bin/$pkgname
 rm -r $pkgdir/usr/share/doc
}
