Kernel for Debian 


```
sudo apt update
sudo apt install devscripts equivs -yq
yes | sudo mk-build-deps -i
DEB_BUILD_OPTIONS=noautodbgsym sudo dpkg-buildpackage -b -Zgzip
```
