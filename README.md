# HNL Project

- [HNL Project](#hnl-project)
  * [Welcome](#welcome)
  * [Analysis Files](#analysis-files)
  * [Editing the repository](#editing-the-repository)

## Welcome
This is the code used for the project titled: [Towards Vertexing Studies of Heavy Neutral Leptons with the Future Circular Collider at CERN](http://urn.kb.se/resolve?urn=urn:nbn:se:uu:diva-444997) by Rohini Sengupta, defended in June 2021. 


## Analysis Files 
This concerns the analysis files [gen_distributions_delphes.py](gen_distributions_delphes.py) and [analysis_HNL_read.py](analysis_HNL_read.py) for HNL analysis at the FCC-ee.

To run gen_distributions_delphes.py a standalone setup created by Suchita Kulkarni (suchita.kulkarni@cern.ch) has to be setup first. 
The setup requires python 3.7 (or higher), Root (version 6.x), PYTHIA8, DELPHES with FastJet and MadGraph.
The input for the gen_distributions_delphes.py analysis file is the HNL sample created by running the wrapper (mg5 + pythia8 + delphes)
from the standalone framework. 

The gen_distributions_delphes.py file is used to validate and analyze the HNL sample. It validates the sample by checking the time 
distribution and the transverese displacement of the sample. The analysis provides studies on the kinematics of the HNL and its 
daughter particles. 

The analysis_HNL_read.py file is an adaptation from the original read_EDM4HEP.py file which provides a basic example showing how to read 
different objects from the EDM4HEP files and how to access and store some simple variables in an output ntuple. The analysis_HNL_read.py 
file is specific for the study of HNLs. It presents a possibility to validate created HNL samples by checking the lifetimes and transverse 
displacements of the samples and also presents the starting point for HNL vertex analysis.

To run the analysis_HNL_read.py file the FCC framework has to be setup following the instructions from the official FCCAnalysis page 
from GitHub. The repositories of interest are the FCCAnalysis and the FCCeePhysicsPerformance. It is very important to make sure that the 
sourcing is correct. For FCCAnalyses, the sourcing should point to the personal FCCAnalyses and not the central version. FCCAnalyses also 
needs to be  linked against FCCeePhysicsPerformane, instructions for which can be found on the respective GitHub pages.


## Editing the repository
This file is markdown (see the extension of this file, '.md'), you can learn a bit more on what markdown can do, you can check the [GitHub markdown guide](https://guides.github.com/features/mastering-markdown/), and also my favorite place, [CodiMD](https://codimd.web.cern.ch/). 

Since it is for documentation, no need for branches, so we send everything to the main branch.

You can edit directly in the browser using the pencil:

![Pencil blue](pencil.png?raw=true "Pencil in blue")

When you are done, you just go down in the page and click the green button that says "Commit changes". 

Or you can copy the repository to a folder in your computer or the lxplus using the following commands.
The first time you need to clone the repository:

`git clone https://github.com/HNL-FCCee/Displaced-HNL-Project `

`cd Displaced-HNL-Project`

Then, inside the folder you can add new files or work in what is there. To add new files, you either just move them there, or create them and edit them normally inside the folder. When you are ready to upload your changes, this is what you have to do.
If you have new files:

`git add nameofthenewfile.extensionofthenewfile`

And then:

`git commit -am "Whatever message to explain your commit"`

`git push`

That is it, this is the simplest, most bare-bones use of a github repository.
