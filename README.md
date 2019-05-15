# Building Autoencoders in Keras

Using https://blog.keras.io/building-autoencoders-in-keras.html as a template, this project is for building simple autoencoders for image denoising

## Set up your environment

First things first, you'll need your environment set up correctly. 

You can follow the instructions here: https://www.youtube.com/watch?v=tfGJlO9AeXU 
This video will walk you through creating your own anaconda environment from this repository: https://gitlab.rc.uab.edu/rc-data-science/horovod-environment

## Cloning the repository

```
#!/bin/bash
# JOB HEADERS HERE
mkdir -p /data/user/$USER/rc-dsc

FOLDER = /data/user/$USER/rc-dsc/building-autoencoders-in-keras
URL = https://gitlab.rc.uab.edu/rc-data-science/building-autoencoders-in-keras.git

if [ ! -d "$FOLDER" ] ; then
    git clone "$URL" "$FOLDER"
else
    cd $FOLDER
    git pull "$URL"
fi

```




