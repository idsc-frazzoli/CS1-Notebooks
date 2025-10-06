# CS1-Notebooks 2025

This GitHub repository contains the Jupyter notebooks associated with the [Control Systems I](https://idsc.ethz.ch/education/lectures/control-systems-i.html) course - taught by [Prof. Emilio Frazzoli](https://idsc.ethz.ch/research-frazzoli/people/person-detail.MjI0MDM0.TGlzdC8yNjg5LDQ4ODg4MTE2Mw==.html) during the fall semester 2025.


## Getting Started with Notebooks

Jupyter notebook is a web-based interactive computing platform. It provides a means to combine live code with narrated text and visualisations. 

Throughout this course, Jupyter notebook(s) will be provided as a means to support and reinforce the concepts introduced in the lectures. Namely, these can be thought of as an interactive alternative to lecture notes and theory sheets. 

We support two ways of using (Jupyter) notebooks:

1. <u>Downloading and running the notebooks locally</u>. Download the files locally, and then run them using a web browser or VS Code. (Note that integrations with other IDEs exist, but we will not support them officially).
2. <u>Using MyBinder</u>. Click on the link in Moodle and run them directly for there.

Note that the first option will usually result in a smoother experience, especially with interactive plots.

## Option 1: Local Installation

### 1. Downloading the Notebooks

To get started with the course materials, you'll need to download the notebooks to your local machine. Follow one of these two methods:

**A. Moodle**

1. Navigate to the course page on Moodle.
2. Locate and download the weekly ZIP file containing the notebook.
3. Move the ZIP file to a suitable directory (location) on your computer for the notebooks.
4. Unzip the file and continue with Step 2 - Setting up the environment. 

**B. GitHub**

1. Click on the link to the CS1-Notebooks repository on GitHub through the course page on Moodle.
2. Click the green `Code` button near the top of the page.
3. In the dropdown menu, click `Download ZIP`.
4. Once downloaded, extract the ZIP file to your chosen directory.

Alternatively, if you prefer using the command line:

```bash
git clone https://github.com/idsc-frazzoli/CS1-Notebooks.git
cd CS1-Notebooks
```

**NOTE**: when using ``git clone``, the cloned repository will be placed within the current directory. 

### 2. Setting up the environment

**Windows**

1. Install Python from the [official Python website](https://www.python.org/downloads/). You need Python version 3.9 or higher.
2. Open Command Prompt and navigate to the project directory.
3. Create a virtual environment:

        python -m venv venv

4. Activate the virtual environment:

        .\venv\Scripts\activate

5. Install Jupyter:

        pip install jupyter

**Linux and MacOS**

1. Install Python (version > **3.9**) by downloading it from the [official Python website](https://www.python.org/downloads/), or using a package manager (e.g., `apt` for Ubuntu, `brew` for macOS).
2. Open a terminal and navigate to the project directory:
   [Terminal navigation tutorial](https://frontend.turing.edu/lessons/module-1/getting-around-in-the-terminal.html) provides a quick introduction to terminal navigation. 
3. Create a virtual environment:

        python3 -m venv venv

4. Activate the virtual environment:

        source venv/bin/activate

5. Install required dependencies:

        pip3 install -r requirements.txt

6. Setup jupyter kernel

        python3 -m ipykernel install --user --name=venv

### 3. Running the Notebooks

To run the notebooks, you can choose between two options:

**A. Using the Notebooks with a web-editor**
Jupyter notebooks - this finds all notebooks within the current directory and trusts them. 

    find . -name '*.ipynb' -exec jupyter trust {} \;

The below runs the notebook. 

    jupyter notebook

**B. Using the notebooks with VSCode**
Install VSCode (if not already present), then:
1. Install the `Python` and `Jupyter` extensions for VSCode. 
2. Choose the python interpreter. Press `Ctrl+Shift+P` and select `Python: Select Interpreter`. Select the `venv` interpreter.
3. Open a notebook file (`.ipynb`). 
4. Choose jupyter kernel. Press `Ctrl+Shift+P` and select `Notebook: Select Notebook Kernel`.
5. Then select `Jupyter Kernel`, and select the kernel `venv` should be present. 
6. You should be able to run the cells from within VSCode. 

## Option 2: Google Colab

Alternatively, if you prefer not to install any software, MyBinder offers a convenient alternative. Simply click on the respective link, wait for the page to load, and then you will be able to run the code.

| Tool name | MyBinder link |
|------------|---------------|
| **LTI Matrix and ODE** | [![Binder]([https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/your-username/your-repo/branch?labpath=time_response_tool%2FODE_LTI.ipynb](https://mybinder.org/v2/gh/idsc-frazzoli/CS1-Notebooks.git/HEAD?urlpath=%2Fdoc%2Ftree%2Ftime_response_tool%2FMenu_Tool.ipynb)) |
| **Root Locus** | Coming soon |
| **Bode plot** | Coming soon |
| **Nyquist plot** | Coming soon |
