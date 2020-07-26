# Aim
This project aims to generate a standardised folder structure to organise, store and re-use experimental data and their analysis results.

# Basic structure
1. Each project is given a folder.
2. Under the project folder, there are
  1. A '**README**' index file that contains

    * A description of the project, such as hypothesis, aim, start date, comments, authors.
    * A list of summary, which lists the most important experiments in bulletins.
    * A full list of experiment folders followed by very short descriptions of each.
  2. A series of **experiment folders**, in the format of '\<ProjectAbbreviation\>_Date_\<Subtype\>', which store

    * Raw data.
    * Metadata file, which explains the protocol of this experiment in details.
    * [Optional] A summary file that summarises the data in this experiment, such as the quatification data directly from image processing.
  3. An '**Analysis**' folder which stores analysis results, which contains:

    * a master **summary file**, in the format of either a LaTex or ppt or plaintext, that summarises all main results as much as possible. Methods to summarise data directly in a LaTex file is in process.
    * [Optional] A '**Tool**' folder, which stores the scripts or any common methods used for data processing for this particular project.  

# Notes
Personally, I very much like using Atom with this framework. I can open the project folder in Atom and the structure will show up on the left. Many analysis and summary in markdown language can be easily done within Atom, without opening multiple windows (notably Jupyter Notebook!) and software. And version control can be easily implemented. I am very new to this and very excited to explore more features!
