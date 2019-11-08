# Python-AI-Arts
AI in Python that converts selected image into the same image in an art style of another selected image.

## Setup
### Install python
```
sudo apt install -y python python-dev python3.6 python3.6-dev python3.7 python3.7-dev python-tk protobuf-compiler 
sudo apt install -y python-pip python3-pip 
sudo apt-get install -y python3 python-dev python3-dev \
     build-essential libssl-dev libffi-dev \
     libxml2-dev libxslt1-dev zlib1g-dev \
     python-pip
sudo apt-get install -y python-h5py
sudo apt-get install -y python3-h5py
sudo apt install -y python-apt
sudo apt install -y python3-apt
```
### Upgrade setuptools
Install testresources
```
pip3 install testresources
```
Then upgrade setuptools
```
pip3 install --upgrade setuptools
```
### Install the dependencies
```
sudo apt-get install -y libpng-dev libtiff-dev libwebp-dev xcftools
pip3 install sklearn
pip3 install numpy
pip3 install argparse
pip3 install h5py
pip3 install keras
pip3 install conda
pip3 install pillow
pip3 install theano
pip3 install imread
pip3 install scipy
pip3 install scikit-image
pip3 install tensorflow
```
## Usage

There are 3 images to identify when we run the script

1. Your base image (to artify)
2. Your reference image (the art to learn from)
3. Your generated image

Run the following comand to generate an image in your chosen style
```
python3.6 Network.py "/path/to/content image" "path/to/style image" "result prefix or /path/to/result prefix"
```
Example
```
python3.6 Network.py ~/Pictures/AIArtConversion/scotland-castle.jpg ~/Pictures/AIArtConversion/modernism.jpg ~/Pictures/AIArtConversion/result.jpg
```
It will go and do 10 iterations, it will take some time so be patient.

Here are some sample results. To see them go to [this link.](https://mega.nz/#F!f9tTQKrI!QWYYvLEzRpvd8Mjn5Jt9iw)
## Convolutional Network Used
[VGG16](https://www.mathworks.com/help/deeplearning/ref/vgg16.html)

[VGG19](https://www.mathworks.com/help/deeplearning/ref/vgg19.html)

[Very Deep Convoltional Networks for Large-Scale Image Recognition by Karen Simonyan & Andrew Zisserman](https://arxiv.org/pdf/1409.1556.pdf)

Karen Simonyan & Andrew Zisserman. Very Deep Convoltional Networks for Large-Scale Image Recognition. PDF file. April 10 2015
https://arxiv.org/pdf/1409.1556.pdf
