# Commands 

## download gitignore using curl 
```bash 
curl https://raw.githubusercontent.com/c17hawke/general_template/main/.gitignore
```
## donload init_setup using curl 
```bash 
curl https://raw.githubusercontent.com/c17hawke/general_template/main/init_setup.sh
```
## Tensorflow verification  

```bash
python -c "import tensorflow as tf;print(tf.config.list_physical_devices('CPU'))"
```
## Instalation of Object Detection API

## Create a Tensorflow Directory 
```bash 
mkdir Tensorflow && cd Tensorflow
```
## Clone the Tensorflow models folder 
```bash
git clone https://github.com/tensorflow/models.git
remove .git file from models  repository to avoid git conflicts
add models folder to .gitignore
```bash
echo "TensorFlow/models" >> .gitignore
```
## run python code
```python
import os 
os.chdir() 
````
## Protobuff Installation/Compilation
- Visit the link - https://github.com/protocolbuffers/protobuf/releases
  - Windows users -
     Search for - protoc-3.20.1-win64.zip
  - Mac users - 
     Search for - protoc-3.20.1-win64.zip 
  - Linux users - 
    Search for - protoc-3.20.1-linux-x86_64.zip
- Unzip into root folder and add '<PATH TO protoc folder>/bin' into system environment variable

- run the following command 
```bash
cd Tensorflow/models/reserch
protoc object_detection/protos/*.proto --python_out=.
```
## Install COCO API
```bash 
pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
```
## Install Object Detection API 
```bash
cp object_detection/packages/tf2/setup.py .
```
## Test your Installation
```bash 
python object_detection/builders/model_builder_tf2_test.py
```

