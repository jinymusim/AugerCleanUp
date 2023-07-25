# Fast Setup to VSCODE for Auger

Data location at https://opendata.auger.org/  

## VSCODE Setup

Download VSCODE https://code.visualstudio.com/download  
Download Git https://git-scm.com/download/win  
During Git Installing, change the editor to VSCODE  
Reaload VSCODE
In Source Control, connect your github with VSCODE  
On Web create Git Archive and clone it to your PC

## Extensions  

Install Python if needed  
Install Python and Jupyter Extensions in VSCODE  
If wanted install other usefull extensions (Pylance, GitLense and other)

## Auger Data Analysis

In https://opendata.auger.org/analysis.php Downlad Notebooks and necessary Datafiles (Summary, Auxiliary, JSON)  
Place the raw .zip files to your Git Archive  
Create new file .gitignore and write *.zip to it so the data is not pushed to Git (TOO BIG!)  
If not installed, install these python packages: **ipykernel, pandas, scipy, numpy, matplotlib, astropy, ipywidgets**  
If possible try to install **healpy**, but it may not work (As consequence **anisotropy.ipynb** won't work)  
If on Windows Machine in function AugerLoad, `replace os.path.join(fdir,file)` with `Path(fdir).joinpath(file).as_posix()`
and add `from pathlib import Path` to the top of the cell.
