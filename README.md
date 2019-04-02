# Open CV setup on Ubuntu

This was to set up my computer with OpenCV 4

```bash
Distributor ID: Ubuntu
Description:    Ubuntu 18.10
Release:        18.10
Codename:       cosmic
```

## Install Dependencies

```bash
sudo apt-get install build-essential
sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev
sudo apt-get install python-dev python-numpy libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libdc1394-22-dev
```

## Clone and Compile Open CV

```bash
git clone git@github.com:opencv/opencv.git
cd opencv/
mkdir opencv-compiled
cd opencv-compiled/
cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..
```

### Using CLion

* After the above steps, open the CMakeLists.txt in this repo.



### References

* https://docs.opencv.org/2.4/doc/tutorials/introduction/linux_install/linux_install.html#linux-installation
* https://docs.opencv.org/2.4/doc/tutorials/introduction/linux_gcc_cmake/linux_gcc_cmake.html