To correctly build this snap you need the following PPAs:

 * ppa:ci-train-ppa-service/landing-011
 * ppa:ubuntu-raspi2/ppa
 * ppa:a-j-buxton/qt5-raspi-eglfs

All Qt build packages must be installed from these PPAs, as well
as Raspberry Pi development files.

See https://launchpad.net/~a-j-buxton/+archive/ubuntu/qt5-raspi-eglfs

Give it an RSS feed, eg:

qmlrss http://feeds.bbci.co.uk/news/rss.xml

Blockers:

 * Need an interface for Broadcom VCHIQ.
   - https://bugs.launchpad.net/snappy/+bug/1533265
 * Need a way to specify PPA dependencies in the snapcraft.yaml.
   - https://bugs.launchpad.net/snapcraft/+bug/1612809
