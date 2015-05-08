# 1.2.2
  * Ruby switch is back!  It has been added to the BrightBox repo (https://github.com/brightbox/deb-ruby2.1/issues/9#issuecomment-69098657)

# 1.2.1
  * Fix character encoding issues in documentation (https://github.com/mojolingo/brightbox-ruby-cookbook/pull/3)

# 1.2.0
  * Default to not installing ruby_switch on 14.x and later since it has been removed. See further details:
    * http://askubuntu.com/questions/452243/what-versions-of-ruby-are-supported-in-14-04/457699#457699
    * https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=737782
    * https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=741050
    * https://launchpad.net/ubuntu/+source/ruby-switch/+publishinghistory
    * https://github.com/mojolingo/brightbox-ruby-cookbook/pull/2

# 1.1.1
  * Remove loading of chef in metadata.rb
  * Test on Ubuntu 14.04

# 1.1.0
  * Allow forcing a different version of Rubygems than that included in the package

# 1.0.0
  * First release
