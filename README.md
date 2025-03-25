# Einführung in das Maschinelle Lernen
Code-Repository für den Kurs "Einführung in das Maschinelle Lernen" an der Hochschule Karlsruhe.

## Install Conda

The recommended way to setup your development environment is to use Miniconda:
### Linux:
Simply run:
```
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh
```
### Windows:

1. Download and install Miniconda from [here](https://www.anaconda.com/download/success)

2. On Windoes, start the `Anaconda Prompt` . On Mac or Linux, just open a new terminal window.

## Setup Conda

The following steps are now similar in both OS:

3. Create a new environment for this course:

    `conda create --name ml-course python=3.8`

4. Activate this environment:

    `conda activate ml-course`

5. Install the following packages: numpy, pandas, matplotlib, scikit-learn.

    `conda install numpy pandas matplotlib scikit-learn jupyter seaborn`

6. Test your installation by opening a new jupyter notebook. A new browser window should open.

    `jupyter notebook`

## Get Code Repository

1. Go to [`https://github.com/pabair/ml-kurs-ss25`](https://github.com/pabair/ml-kurs-ss25)

2. Copy the URL of the new Repository

3. In a Terminal, run:  `git clone [URL of repo]`

4. Change into the directory: `cd ml-kurs-ss25`

5. (later) As the original repository gets updated, run `git pull` in the terminal to fetch the changes from Github to your computer

## Alternative Setup in Linux / Windows Subsystem for Linux (WSL)

If you don't want to use Conda, you can also install the packages using pip in a virtual environment:

1. Create a new virtual environment:

    `python3 -m venv venv/`

2. Activate the environment:
    
    `source venv/bin/activate`

3. Install the packages:
   
    `pip install -r requirements.txt`

4. Start the Jupyter Notebook with `jupyter notebook .`

Instead of `jupyter notebook`, you can also open the project in VSCode (with the Jupyter extension installed) by running `code .` in the terminal and then selecting the venv as the Python interpreter for Jupyter.