# Maintainer: Alexander Georgievskiy <galeksandrp@gmail.com>

pkgname=lib32-ffmpeg-steam
pkgver=0.1.0
pkgrel=3
pkgdesc='ln -s /usr/lib32/libav*.so* /home/*/.local/share/Steam/ubuntu12_32/libav*.so* (fix VAAPI memleak for Steam)'
arch=(x86_64)
url='https://freedesktop.org/wiki/Software/vaapi'
license=('MIT')
depends=(lib32-ffmpeg-compat-57 steam)
makedepends=()
optdepends=()
source=('lib32-ffmpeg-steam-libx.path'
        'lib32-ffmpeg-steam-libx.service'
        'lib32-ffmpeg-steam.service'
        'streaming_client_ld')
sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

package() {
  install -D ../lib32-ffmpeg-steam-libx.path "${pkgdir}/usr/lib/systemd/user/lib32-ffmpeg-steam-libx.path"

  install -D ../lib32-ffmpeg-steam-libx.service "${pkgdir}/usr/lib/systemd/user/lib32-ffmpeg-steam-libx.service"

  install -D ../lib32-ffmpeg-steam.service "${pkgdir}/usr/lib/systemd/user/lib32-ffmpeg-steam.service"

  install -D ../streaming_client_ld "${pkgdir}/usr/bin/streaming_client_ld"
}
