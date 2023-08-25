

![egusphere image](https://github.com/saraemp/egusphere-2023-53_private/blob/master/3_postprocessing/Figures/images/readme_image.png)

# The flexural isostatic response of climatically driven sea-level changes on continental-scale deltas 

This repo looks at a series  of  conceptual  simulations  to investigate flexural isostatic responses to high-frequency fluctuations in water and sediment load associated with climatically driven sea-level changes.  Te simulation models a large drainage basin that discharges to a continental margin to generate a deltaic depocenter, then prescribe synthetic and climatic-driven sea-level curves of different frequencies to assess flexural response. 

Results show that flexural isostatic adjustments are bidirectional over 100-1000 kyr timescales and are in sync with the magnitude, frequency, and direction of sea-level fluctuations, and that isostatic adjustments play an important role in driving along-strike and cross-shelf river-mouth migration and sediment accumulation. 

## Files to Run
To keep the figures consistent with the research article published with this package, you can use the data and the extracted_results folder to run your scripts

The script can be run using Jupyter Notebook.  The test for the package can be done with the notebooks;
 "3_postprocessing/Figures/Fig_3d.ipynb" or "3_postprocessing/Figures/Fig_6.ipynb" 
 
##  Running model via Docker
In order to reproduce the full model results you will need to re-run the model.  The simplest way to do this is via using the badlandsmodel docker image.  
1. Download and install docker desktop from :  https://docs.docker.com/desktop/
2. Follow the instruction on https://badlands.readthedocs.io/en/latest/install.html to initialize the badlands model within docker.  The following commands can be used in Linux or Mac environments;
    1. docker pull badlandsmodel/badlands
    2. docker run -it -p 8888:8888 -v "$PWD":/live/share badlandsmodel/badlands
3. Now you will need to download, navigate to and open this repository from your local machine within the docker environment.  The easiest way to do this is with github;
    1. Download and install Git on your machine from https://github.com/git-guides/install-git
    2. Open a terminal (command prompt in windows) and clone this repo with the command -> "git clone https://github.com/saraemp/egusphere-2023-53_private.git"
4. Start Docker and open Project 
    1. Copy and paste the address "localhost:8888" in your browser of choice to start docker. 
    2. Open the folder called "share"  (This will have all your files from your home directory) 
    3. Navigate to wherever you have cloned the git repository
    4. Open the folder 2_model_runing (this has the model configuration and paramaters preset for you)
    5. Open the notebook "Run.ipynb" and execute the model
    
## Running model locally
You will need to install the dependencies necessary to run the package.  Conversely, you can  use the command 

"pip install -r requirements.txt"

All the dependencies required to run the package is listed in the requirements.txt file.  

## Citing this package
S. Polanco et al., “The flexural isostatic response of climatically driven sea-level changes on continental-scale deltas,” EGUsphere, vol. 2023, pp. 1–30, 2023, doi: 10.5194/egusphere-2023-53.

## Link to publication 
https://egusphere.copernicus.org/preprints/2023/egusphere-2023-53/


