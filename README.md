# NREL Sectral Efficiency and Tandem calculator
This is a wrapper around the [`NREL SE and Tandem` package](https://github.com/NREL/SE-and-Tandems) designed for easier installation and use. The package is included as a Git submodule (https://git-scm.com/book/en/v2/Git-Tools-Submodules).

## How to use

### Installation
1. Clone this repo by running
```sh
git clone --recurse-submodules https://github.com/uni-stuttgart-ipv/nrel_se_and_tandems.git`
```
in your command line to download the package.
Git will create a new folder called `nrel_se_and_tandems` in the folder you are in in the command line.
Move into the projet folder by running
```sh
cd nrel_se_and_tandems
```

2. (optional, but recommended) Create a [Python virtual environment](https://docs.python.org/3/library/venv.html) for this project. 
Virtual environments are isolated Python instances so you don't have to worry about anything you do within it affecting any other Python projects on your computer.
To create and activate the virtual environment run
```sh
python -m venv .venv
.venv/Scripts/activate
```
> Note: You have to activate the virtual environment any time you want to use this project. 
When activated you sould see `(.venv)` written on the left of your terminal window.

3. Install the required dependencies 
```sh
pip install requirements.txt
```
from the command line to install all dependencies.

### Spectral Efficiency (SE)
1. Open [SE_Calculation_GUI.ipynb](./SE-and-Tandems/notebooks/SE_Calculation_GUI.ipynb).
2. Run all the cells until the GUI opens.
3. Select the IV, EQE, and spectrum to calculate (Example data in [Examples/SE](./SE-and-Tandems/Examples/SE/)).

### Tandem performance
1. Open [Tandem_Performance_GUI.ipynb](./SE-and-Tandems/notebooks/Tandem_Performance_GUI.ipynb).
2. Run all the cells until the GUI opens.
3. Select the top cell, bottom cell, and coupling method to use (Example data in [Examples/Tandem Performance](<./SE-and-Tandems/Examples/Tandem Performance/>)).
4. Calculate the results using one of the terminal options.

## Updating the NREL SE and Tandem package submodule
To update the original NREL package run
```sh
git submodule update --remote
```
from the command line.
If updates are available please `commit` them.

## Resources
+ [Walkthroughs](./SE-and-Tandems/Examples/PDF_walkthroughs/)