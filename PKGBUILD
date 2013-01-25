pkgname=dwm
pkgver=6.0
pkgrel=1
pkgdesc="A dynamic window manager for X"
url="http://dwm.suckless.org"
arch=('i686' 'x86_64')
license=('MIT')
depends=('libxinerama' 'pango')
options=(zipman)
provides=('dwm')
conflicts=('dwm-pango')
_source=(http://dl.suckless.org/dwm/dwm-$pkgver.tar.gz
        config.h)
_patches=(00-${pkgname}-${pkgver}-buildflags.diff
		  01-${pkgname}-${pkgver}-xft.diff
		  02-${pkgname}-${pkgver}-pertag2.diff
		  03-${pkgname}-${pkgver}-systray.diff
		  04-${pkgname}-${pkgver}-statuscolors.diff
		  05-${pkgname}-${pkgver}-occupiedcol.diff
		  06-${pkgname}-${pkgver}-no_title.diff)
		  #07-${pkgname}-${pkgver}-single_window_no_border.diff

source=(${_source[@]} ${_patches[@]})

build() {
  for PATCH in "${_patches[@]}"; do
    msg "${PATCH##*/}" && patch -Np1 -i "${startdir}/${PATCH##*/}"
  done

  cd $srcdir/$pkgname-$pkgver
  cp $srcdir/config.h config.h

  make X11INC=/usr/include/X11 X11LIB=/usr/lib/X11 || return 1
  make PREFIX=/usr DESTDIR=$pkgdir install || return 1

  install -m644 -D LICENSE $pkgdir/usr/share/licenses/$pkgname/LICENSE && \
  install -m644 -D README $pkgdir/usr/share/doc/$pkgname/README
}
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '777d39eea2a64b4a855432da59f303fe'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'e4610156be4106b3b52fb38fa865ac10'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'a5abdc26a64f14ebee6b26b352901a61'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'eafdf1ace28b028b46c256e8f2b27486'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'eafdf1ace28b028b46c256e8f2b27486'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'd5f678c6c6b3ffa45c3d8aef19ef84dd'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '60030ce7c632df3052027c998120e1fa'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2c7e18580a460465d6e6095944530e7d'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '60030ce7c632df3052027c998120e1fa'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '39dc4cf010cc9986a49d080cead96860'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '2378629720710f88268efaad315ec81b'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '6fbd2b8cbc42afb04e68a306173a9297'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         'f79fb280b5632a4c19e5ce42001066f5'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
md5sums=('8bb00d4142259beb11e13473b81c0857'
         '35d8f538fcdf0e30985ca3fbb5fb92e5'
         '0980b328204a1f8d0664a413510c450a'
         '951dfa6139e99e8bbcdf999ba182803b'
         '0fd771ad51b80c3872c9080bd15f6eea'
         '6a0f657a18b77764fdd70a819b78412f'
         '5de666a41912731a9fa0ab40d5c497e0'
         '5ea175f007b04b82befa36d3c139db04'
         'd87223a0c056e59a0dd6a5fba5d0c745')
