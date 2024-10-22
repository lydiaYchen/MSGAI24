# MSGAI lab innstructions

## Course Overview
This course covers the fundamentals and applications of generative AI.

The lab consists of three parts, each with two group tutorial sessions to be given by the TAs and one individual homework to be solved by students.

- Part 1: [Fine-tuning Generative Models](#part-1-diffusion)
    - Tutorial 1A - Fine-tuning diffusion
    - Tutorial 1B - Sampling of diffusion 
    - Homework 1 
- Part 2: [Benchmarking Generative Models](#part-2-large-language-models)
    - Tutorial 2A - Prompt design (+Sampling)
    - Tutorial 2B - Few-Shot (+Sampling) / Fine-tuning of LLM
    - Homework 2 
- Part 3: Modeling of Generative Models
    - Tutorial 3A - Solving DTMC
    - Tutorial 3B - Solving CTMC
    - Homework 3 
    

## Part 1: Diffusion
We will **NOT** provide any technical assistance during the lab, please refer to the internet or other students for questions regarding your setup.

### Prerequisites

You need to have access to a computer able to load the different models we are going to use. All the code will be run on your personal computer.

Alternatively you can use [colab](https://colab.google.com) to run the different notebooks, but be aware of the limitations implied.

### Technical requirements

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

## Part 2: Large Language Models
We will **NOT** provide any technical assistance during the lab, please refer to the internet or other students for questions regarding your setup.

### Prerequisites

You need to have access to a computer able to load the different models we are going to use. All the code will be run on your personal computer.

Alternatively you can use [colab](https://colab.google.com) to run the different notebooks, but be aware of the limitations implied.

> This Lab and HW will make use of a small LLM, which benefits greatly from an accelerator like GPU or Intel IPEX (e.g.,
for (scalable) Xeon, consumer, and Xe+ graphics.). The GPUs from Google Collab should be more than sufficient for this
model.


> ⚠️ Before attending the lab, make sure you have run the first set of cells in [`homework_llm.ipynb`](homework_llm.ipynb),
this will ensure that you have: 1) Downloaded the dataset (`standford/imdb`) for sentiment analysis, and 2) Downloaded the
model (`google/flan-T5-small`), that you will use during the lab and the HW.


### Technical requirements

The code will be written in **Python** using **Pytorch** and **Transformers** from 🤗 **Huggingface** for the experiments.
The lab is designed to run on Linux or a similar platform. We provide the environment required in the file [llm_env.yml](llm_env.yml),
and [llm_env-cuda.yml](llm_env-cuda.yml), for CPU and CUDA enabled platforms respectfully.

Once you have downloaded [conda](https://docs.anaconda.com/miniconda/#miniconda-latest-installer-links), you'll have to set up the environment by running:
````bash
# FOR CPU
conda env create --file=llm_env.yml 
# FOR CUDA
conda env create --file=llm_env-cuda.yml 
````

If you have access to a CUDA compatible GPU, you can use the file [env-cuda.yml](env-cuda.yml) (Make sure you have installed and correctly set up CUDA 12 *with
cuda-toolkit* first).

You'll be able to launch jupyter using:

````bash
# FOR CPU
conda activate msgai-llm
jupyter notebook
````

We will share a notebook at the beginning of each lab, along with the information about the dataset or additional material we'll be using.

### Submitting the Homework to Ilias
**N.B.** To submit this homework, you must render this notebook as a PDF as well as be able to provide the `ipynb` file.
To render the notebook for submission, you are required to run the following command. Make sure to test this command beforehand;

```bash
jupyter-nbconvert --to pdfviahtml  \
  homework_llm.ipynb \
  --TagRemovePreprocessor.remove_input_tags='{"hide-cell","hide-student-submission"}' \
  --TagRemovePreprocessor.remove_all_outputs_tags='{"remove-output"}'         
```

> This command ensures that we get a more compacted PDF, and input and/or output(s) for cells are cleaned-up to ensure
grading.

Before submitting make sure your notebook adheres to the following requirements:

1. None of the cells that are tagged as `keep-output` or `hide-cell` are deleted, these are key for the review of your code.
2. None of the cells that contain a commment along the lines `# Do not edit this cell`, are indeed, not (functionally)
altered.
2. You have verified that your submission PDF contains all your complete answers, note that;
   * cells annotated with `hide-cell` will have their input removed,
   * cells annotated with `remove-output` will have their output removed,
   * cells annotated with `hide-student-submission` will have their input removed, e.g., this cell
3. Any cells you have added are either: properly annotated with `keep-output` or `hide-cell`, or are manually cleaned.

We do recommend using `git` to commit your work, and able to revert breaking changes. In case you do not want to have
a cluttered history with the output of cells, you can use the following git config;

in `$HOME/.gitconfig`, add the following `filter`, which will clean ouput, but keep cell-tags in your git history,
you may wish to alter this to your liking.
```
[filter "strip-notebook-output"]
clean = "jupyter nbconvert --ClearOutputPreprocessor.enabled=True --ClearMetadataPreprocessor.enabled=True  --ClearMetadataPreprocessor.preserve_cell_metadata_mask='[(\"tags\")]' --to=notebook --stdin --stdout --log-level=ERROR"
```

And create a [`../.gitattributes`] file, containing/appending the following line. This will ensure that the filter from your
`.gitconfig` will be run for all jupyter notebooks.
```
*.ipynb filter=strip-notebook-output
```
