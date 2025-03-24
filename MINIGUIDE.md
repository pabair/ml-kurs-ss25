## Install Miniconda

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

The following steps are similar in both OS:

1. Create a new environment for this course:
   
    `conda create --name ml-course python=3.8`

2. Activate this environment:
    
    `conda activate ml-course`

3. Install the following packages: numpy, pandas, matplotlib, scikit-learn.
    
    `conda install numpy pandas matplotlib scikit-learn jupyter seaborn`

4. Test your installation by opening a new jupyter notebook. A new browser window should open.
    
    `jupyter notebook`


## Get Code Repository

1. Go to [`https://github.com/pabair/ml-kurs-ss25`](https://github.com/pabair/ml-kurs-ss25)

2. Click Fork button and create a fork

3. Copy the URL of the new Repository

4. In a Terminal, run:  `git clone [URL of repo]`

5. Change into the directory: `cd ml-kurs-ss25`

6. (later) As the original repository gets updated, you can "sync the fork" in Github using the button. Then, in the terminal, run `git pull` to fetch the changes from Github to you computer.

You can now make edits in your own copy of the code 

## Run the examples

Reopen the anconda prompt and run: `jupyter notebook ml-kurs-2025`, the directory will open in a Jypter Notebook.