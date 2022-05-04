# Commands 

## gownload gitignore using curl 
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
```
## run python code
```python
import os 
os.chdir() 
````
##    

