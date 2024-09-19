# MSGAI lab requirements

## Course Overview
This course covers the fundamentals and applications of generative AI. Detailed program of the labs is available in the Instruction file.

We will **NOT** provide any technical assistance during the lab, please refer to the internet or other students for questions regarding your setup.

## Prerequisites

You need to have access to a computer able to load the different models we are going to use. All the code will be run on your personal computer.

Alternatively you can use [colab](https://colab.google.com) to run the different notebooks, but be aware of the limitations implied.

## Technical requirements

The code will be written in **Python** using **Pytorch** for the experiments. The lab is designed to run on Linux or a similar platform. We provide the environment required in the file [env.yml](env.yml).
Once you have downloaded [conda](https://docs.anaconda.com/miniconda/#miniconda-latest-installer-links), you'll have to set up the environment using
````bash
conda env create --file=env.yml 
````

If you have access to a CUDA compatible GPU, you can use the file [env-cuda.yml](env-cuda.yml) (Make sure you have installed and correctly set up CUDA 12 first).

You'll be able to launch jupyter using:

````bash
conda activate msgai
jupyter notebook
````

We will share a notebook at the beginning of each lab, along with the information about the dataset or additional material we'll be using.

