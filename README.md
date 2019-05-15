# Building Autoencoders in Keras

Using https://blog.keras.io/building-autoencoders-in-keras.html as a template, this project is for building simple autoencoders for image denoising

## Set up your environment

First things first, you'll need your environment set up correctly. 

You can follow the instructions here: https://www.youtube.com/watch?v=tfGJlO9AeXU 
This video will walk you through creating your own anaconda environment from this repository: https://gitlab.rc.uab.edu/rc-data-science/horovod-environment

## Cloning the repository

1. Use the Job Composer at https://rc.uab.edu/pun/sys/myjobs/workflows
2. Create a new job from the default template
3. Scroll down and click "Open Editor" 
4. Copy and paste the script below into over the current contents

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

## Starting up the notebook

You can start up an interactive Jupyter notebook session through rc.uab.edu to check if the environment works.

Under environment setup, specify

```
# Load required modules
module load cuda10.0/toolkit
module load Anaconda3


```

Under Extra jupyter arguments, specify

```
--notebook-dir=/data/user/$USER/rc-dsc/building-autoencoders-in-keras
```

For partition, specify

```
pascalnodes
```

If you run into any problems with the code or setup, feel free to come to our weekly office hours listed on the website: https://www.uab.edu/it/home/research-computing








