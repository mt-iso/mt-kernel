Kernel for Debian 


```
sudo apt update
sudo apt install devscripts equivs -yq
yes | sudo mk-build-deps -i
DEB_BUILD_OPTIONS=noautodbgsym sudo dpkg-buildpackage -b -Zgzip
```

Debian Experimental depodaki kernel için:

```
echo 'deb https://deb.debian.org/debian experimental main contrib non-free' | sudo tee /etc/apt/sources.list.d/experimental.list && sudo apt update && sudo apt install linux-image-6.7-amd64
```
