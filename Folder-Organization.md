We store project files on both the GitHub repo and a Dropbox folder. 

There is one important principle: all files on GitHub and Dropbox must ultimately be either completed (clean, documented, and checked into the system ready for others to use them) or abandoned (all files deleted), but never left indefinitely in a half-finished state. For storing intermediate work and personal files, you could set up a separate Dropbox folder called ProjectName-Personal.

GitHub and Dropbox have different features, which determine which file types we store on them. GitHub cannot store large files, but it keeps complete version histories and makes it easy to roll back to previous versions. Dropbox can store large files, but it may keep incomplete version histories (depending on your Dropbox account) and makes it difficult to comprehensively roll back to previous versions. We thus store all code and final output files on GitHub, while we store large data files, Powerpoint presentations, as well as some notes, on Dropbox.

### GitHub repository
The GitHub repo has two main folders: Code and Paper. 
* Code/Build contains all data prep code.
* Code/Analysis contains all code to construct tables and figures.
* Code/Tex has the tex files for the paper and Beamer presentations
* Output/Analysis contains ONLY figures and tables for use in the tex files and presentations. 
* Output/Tex contains only the pdfs made by the tex files, e.g. the paper and the presentation.

GitHub likes to keep total storage low, and will not allow users to push files larger than 100MB. If for some reason a code or output file is larger than about 10 MB, then we should store it on Dropbox.

Each subfolder within Code/Build and Code/Analysis should include a batch script (likely in Python) that executes all code in that subfolder in the proper sequence.

### Dropbox
Dropbox stores all data files as well as other project documents.
* dropbox/ProjectName/RawData stores all original data files that are used in the analysis. (If there is a data file that we want to store for possible future use/reference but we are not using in the analysis, we should store it in a separate folder called dropbox/ProjectName/DataStorage/. But ideally all data should be in dropbox/ProjectName/RawData in its original form, so all processing (e.g. unzipping, manipulating, importing into Stata) is done by programs called from the python script MakePaper.py.)
 - All folders containing raw data should have a plain text README file that details the data source and any additional information that is necessary for replication.
* dropbox/ProjectName/IntermediateData stores all intermediate data files, i.e. files created by the code in the GitHub Code folder.
* Admin stores time sheets, data use agreements, etc.
* Literature stores all relevant literature, typically in pdf format. Please use the following format to name files: Authors_ShortTitle_Year.pdf.
* Notes stores any comments or notes that we want to share between each other that are too long or complicated for a post on slack (e.g. a latex file and associated pdf that works through a proof). Very long notes in plain text format (e.g., long latex proofs) could be done in a Notes folder within the Github repo.

### Exploratory work
Especially early in a project, there will be exploratory work that may or may not go into the paper. This work could live in git branches or /Scratch/ subfolders. Please keep this clean: once we are fairly sure that an analysis is not in the paper, it should be removed from the master repo. We can always return to it if needed.

### Code structure
In general, the code in GitHub/.../Code/Build/ will operate on data from dropbox/.../RawData/ and place it in dropbox/.../IntermediateData/. Then code in GitHub/.../Code/Analysis/ will take data from dropbox/.../IntermediateData/ and construct tables and figures to be placed in GitHub/.../Output/Analysis/. We also want to be able to trace dependencies and keep the folders clean of unused files. Thus, to the extent that is reasonable, GitHub/.../Code/Build, dropbox/.../RawData/, dropbox/.../IntermediateData/, and perhaps GitHub/.../Code/Analysis should have parallel structures. For example, these folders might all have a subfolder called "CensusData", so code from GitHub/.../Code/Build/CensusData/ prepares data from dropbox/.../RawData/CensusData/ and puts prepared data in dropbox/.../IntermediateData/CensusData/. 
