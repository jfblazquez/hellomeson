# How to use libraries in meson example

First install meson if not installed

``` console
sudo apt install meson ninja-build
``` 

or with python

``` console
sudo apt-get install python3 python3-pip python3-setuptools \
                       python3-wheel ninja-build
pip3 install --user meson
```

``` console  
mkdir subprojects
meson wrap install fmt
meson setup build
cd build
meson compile
```

More info at https://mesonbuild.com/Using-wraptool.html

Use `meson wrap status` to check if your projects are up to date
Use `meson wrap update fmt` to update fmt library