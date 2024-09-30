# MSGAI lab innstructions

## Course Overview
This course covers the fundamentals and applications of generative AI.

The lab consists of three parts, each with two group tutorial sessions to be given by the TAs and one individual homework to be solved by students.

- Part 1: Fine-tuning Generative Models
    - Tutorial 1A - Fine-tuning diffusion
    - Tutorial 1B - Sampling of diffusion 
    - Homework 1 
- Part 2: Benchmarking Sampling of Generative Models
    - Tutorial 2A - Prompt design
    - Tutorial 2B - Sampling of LLM
    - Homework 2 
- Part 3: Modeling of Generative Models
    - Tutorial 3A - Solving DTMC
    - Tutorial 3B - Solving CTMC
    - Homework 3 
    

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

