# CS1 - 2024 -Notebooks

This GitHub repository contains the Jupyter notebooks associated with the [Control Systems I]([url](https://idsc.ethz.ch/education/lectures/control-systems-i.html)) course - taught by [Prof. Emilio Frazzoli](https://idsc.ethz.ch/research-frazzoli/people/person-detail.MjI0MDM0.TGlzdC8yNjg5LDQ4ODg4MTE2Mw==.html) during the fall semester 2024.


## Getting Started with Notebooks

Jupyter notebook is a web-based interactive computing platform. It provides a means to combine live code with narrative text and visualisations. 

Throughout this course, Jupyter notebook(s) will be provided as a means to support and reinforce the concepts introduced in the lectures. Namely, these can be thought of as an interactive alternative to lecture notes and theory sheets. 

We support two ways of using (Jupyter) notebooks:

1. <u>Download and run the notebooks locally</u>. Download the files locally, and then run them either through the web browser or VS Code. (Note that integrations with other IDEs exist, but we will not support them officially).
2. <u>Using Google Colab</u>.: **todo**



## [Option 1] Local Installation Guide 

### Downloading the notebooks
The first step is to locally download the files within this repository. There are two options:

1. Using git: *maybe remove?*
   1. Ensure that git (version **>2.39?**) is installed by entering `git -v` in the terminal. If not installed, see [Git's official website](https://git-scm.com/downloads) for installation instructions. 
   2. Using the terminal, navigate to the desired directory and clone the repository: ``git clone <<https://address.git>>``
2. Manual download: 
   1. On this page above, click the green `code` button, and then use `Download ZIP`.
   2. Extract the ZIP file to your desired directory.  
 
**NOTE**: Take note of where the files are downloaded. `git clone` will download the files into the current directory. 

### Setting up the environment

**Windows**

**Linux and mac**

1. Install Python (version > **3.9?**) by downloading it from the [official Python website](https://www.python.org/downloads/), or using a package manager (e.g., `apt` for Ubuntu, `brew` for macOS).
2. Open a terminal and navigate to the project directory:
   1. [Terminal navigation tutoral](https://frontend.turing.edu/lessons/module-1/getting-around-in-the-terminal.html) provides a quick introduction to terminal navigation. 
3. Create a virtual environment:

        python3 -m venv venv

4. Activate the virtual environment:

        source venv/bin/activate

5. Install required dependencies:

        pip3 install -r requirements.txt

6. Setup jupyter kernel

        python3 -m ipykernel install --user --name=venv

## [Option a] Using the Notebooks with a web-editor
Jupyter notebooks - this finds all notebooks within the current directory and trusts them. 

    find . -name '*.ipynb' -exec jupyter trust {} \;

The below runs the notebook. 
    jupyter notebook

## [Option b] Using the notebooks with VSCode
Install VSCode (if not already present), then:
1. Install the `Python` and `Jupyter` extensions for VSCode. 
2. Choose the python interpreter. Press `Ctrl+Shift+P` and select `Python: Select Interpreter`. Select the `venv` interpreter.
3. Open a notebook file (`.ipynb`). 
4. Choose jupyter kernel. Press `Ctrl+Shift+P` and select `Notebook: Select Notebook Kernel`.
5. You should be able to run the cells from within VSCode. 

## Option 2: Google Colab

