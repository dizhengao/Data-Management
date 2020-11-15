# Aim
This project aims to generate a standardised folder structure to organise, store and re-use experimental data and analysis results.

# Basic structure
### 1. Each project is given a folder.
### 2. Under the project folder, there are:
1. A '**README**' index file (e.g. the README.txt file in this project) that contains
    * A description of the project, such as hypothesis, aim, start date, comments, authors.
    * A list of summary, which lists the most important experiments in bulletins.
    * A full list of experiment folders followed by very short descriptions of each.
2. A series of **experiment folders**, in the format of '\<ProjectAbbreviation>\_Date_\<Subtype\>', which store
    * Raw data.
    * A metadata file, which explains the protocol of this experiment in details. The metadata files should follow a common structure to be easily transferred into LaTex files. The common structure is illustrated in the '20190618' folder.
    * A 'summary' file that summarises the data in this experiment, such as the quatification data directly from image processing.
3. An '**Analysis**' folder which stores analysis results, which contains:
    * a master **summary file**, in the format of ppt, plaintext or some other format that is easy for storing processed data, that summarizes results from each experiment. The content in this file could be later re-used in LaTex files. 
    * [Optional] A '**Tool**' folder, which stores the scripts or any common methods used for data processing for this particular project.  
4. A '**Latex**' folder which holds a series of LaTex files that give a formal real-time summary for ongoing projects. The main structure is listed below. To see detailed information and what is included in each .tex file please refer to files in the 'Latex' folder. This section is preliminary and more features is being added (especially to make integrating each experiment into the final latex files easier and prettier).
    * [ProjectName].tex: The main .tex file 
    * 1.Introduction.tex: Some introduction literature, thoughts and ideas.
    * 2.Methods.tex: Experimental protocols and analysis methods.
    * 3.Results.tex: The main .tex file that contains results from each experiment and needs to be updated on the move.
    * 4.Summary.tex: Summary of main results; Discussion on results; TO-DO lists.
    * preamble.tex: Inludce packages, define new commands, etc.

### 3. General workflow
For each new experiment, create a folder named with date -> initialize a metadata file -> add raw data -> create a summary file -> update master summary file and README file -> run 'cat' command on BASH to integrate this experiment into LaTex files.

# Notes
Personally I very much like using VS Code with this framework. I can open the project folder in VS Code with the dedicated structure showing on the left. Many analysis and summary in markdown language can be easily done within a single VS Code interface, without opening and switching between multiple windows (notably Jupyter Notebook!) and software. Version control can also be easily implemented. I am still new to this and very excited to explore more features!
