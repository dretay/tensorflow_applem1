# Tensorflow / OpenCV example on Apple M1 Silicon

> An example project to get Tensorflow and OpenCV running on Apple Silicon. 
> Tensorflow compatibility is under active development, so you'll likely need to update the links used in this project. 

### Build Instructions
1. [Download](https://www.anaconda.com/products/individual) and install Conda. There are so many specifics to getting a compatible build, this is kinda a necessity. 
2. Launch Anaconda Navigator
3. Open a terminal in the base (root) environment
4. Create an environment using [environment.yml](foo)
```console 
  conda env create --file=environment.yml --name=YOUR_ENV_NAME
```
5.  Activate that environment
```console
conda activate YOUR_ENV_NAME
```
6. Install tensorflow
```console
pip install --upgrade --force --no-dependencies https://github.com/apple/tensorflow_macos/releases/download/v0.1alpha3/tensorflow_macos-0.1a3-cp38-cp38-macosx_11_0_arm64.whl https://github.com/apple/tensorflow_macos/releases/download/v0.1alpha3/tensorflow_addons_macos-0.1a3-cp38-cp38-macosx_11_0_arm64.whl
```
7. Install OpenCV
```console
conda install -c conda-forge opencv matplotlib
```
8. [Download](http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v2_coco_2018_03_29.tar.gz) the coco pre-trained data set
