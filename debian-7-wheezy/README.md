# devuan-debmirror

* debmirror script modified in order to make a PRIVATE mirror of a devuan package repository
* this script apply for debian wheezy
* this is NOT the official way to make a public mirror and MUST NOT be used to make a public mirror
* see : https://lists.dyne.org/lurker/message/20170802.090410.d78d51fe.en.html
* https://devuan.org

Example : mirroring jessie :

```
debmirror /mirror/devuan/ \
	--host=packages.devuan.org \
	--arch=i386,amd64 \
	--dist=jessie,jessie-backports,jessie-proposed-updates,jessie-security,jessie-updates \
	--omit-suite-symlinks \
	--diff=none \
	--root=merged \
	--verbose \
	--i18n \
	--method=http \
	--keyring /mirror/541922FB.bin
```
