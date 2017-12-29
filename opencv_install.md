```
方法1:
yum -y install http://li.nux.ro/download/nux/dextop/el7/x86_64/nux-dextop-release-0-5.el7.nux.noarch.rpm
yum -y install ffmpeg ffmpeg-devel

yum -y install cmake cmake-gui gstreamer* texlive-bibtex python-beautifulsoup libgphoto2-devel python-devel numpy gcc gcc-c++ gtk2-devel gtk3-devel libdc1394-devel libv4l-devel gstreamer-plugins-base-devel libpng-devel libjpeg-turbo-devel jasper-devel openexr-devel libtiff-devel libwebp-devel tbb-devel eigen3-devel doxygen openblas-devel gtkglext-devel python34-pylint vtk-devel

pip install SQLAlchemy matplotlib numpy

wget https://raw.githubusercontent.com/opencv/opencv_3rdparty/dfe3162c237af211e98b8960018b564bc209261d/ippicv/ippicv_2017u3_lnx_intel64_general_20170822.tgz
下载包到/root/opencv_ljtest/opencv-3.4.0/.cache/ippicv

https://opencv.org

git clone https://github.com/opencv/opencv.git
git clone https://github.com/opencv/opencv_extra.git

mkdir build
cd build
cmake -D WITH_TBB=ON -D WITH_EIGEN=ON -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..

make
make install

ln -s /usr/local/lib/python2.7/site-packages/cv2.so cv2.so

方法2:
yum -y install python34 python34-devel python34-pip
pip3 install opencv-python h5py

测试:
import cv2
print(cv2.__version__)

```
