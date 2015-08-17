# Maintainer: Francois Garillot <francois[@]garillot.net>
# Contributor: Daenyth <Daenyth+Arch [at] gmail [dot] com>
_gemname=text-hyphen
pkgname=ruby-$_gemname
pkgver=1.4.1
pkgrel=1
pkgdesc="Text::Hyphen is a Ruby library to hyphenate words in various languages using Ruby-fied versions of TeX hyphenation patterns"
arch=('any')
url="http://rubygems.org/gems/text-hyphen"
license=('GPL')
depends=('ruby')
makedepends=('rubygems')
source=(http://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
md5sums=('e44f810d85b7ea4d568cd991af364bd9')
sha1sums=('ec45bc4b96a0b094158907a1f1daf638ef131669')

package() {
  cd "$srcdir"
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir$_gemdir" $_gemname-$pkgver.gem
}
# vim:set ts=2 sw=2 et:
