# devuan-debmirror

* debmirror script modified in order to mirror a devuan package repository
* this script apply for debian wheezy

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
