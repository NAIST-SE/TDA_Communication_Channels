# Replication Package: A Topological Analysis of Communication Channels for Knowledge Sharing in Contemporary GitHub Projects

[https://github.com/NAIST-SE/TDA_Communication_Channels](https://github.com/NAIST-SE/TDA_Communication_Channels)

This is a replication package for the paper **A Topological Analysis of Communication Channels for Knowledge Sharing in Contemporary GitHub Projects**.
This artifact is a repository consisting of (a) dataset including (i) 3 files related to RQ1 with the information of Repository Fork?, Repository Forks Count, Repository Issues enabled?, Repository Wiki enabled?, Repository Pages enabled?, Repository Open Issues Count, Repository Readme filename, Repository Changelog filename, Repository Contributing guidelines filename, Repository License filename, Repository Code of Conduct filename, Repository Security Threat Model filename, Repository Security Audit filename, Platform; 
(ii) 7 files related to RQ2 including the information of Repository Fork?, Repository Forks Count, Repository Issues enabled?, Repository Wiki enabled?, Repository Pages enabled?, Repository Open Issues Count, Repository Readme filename, Repository Changelog filename, Repository Contributing guidelines filename, Repository License filename, Repository Code of Conduct filename, Repository Security Threat Model filename, Repository Security Audit filename, Platform, Repository Stars Count;
(b) figure contains all figures of topological data analysis; and 
(c) script, python code used in the research.


## Abstract
With over 28 million developers, success of the GitHub collaborative platform is highlighted through an abundance of communication channels among contemporary software projects. 
Knowledge is broken into two forms and its sharing (through communication channels) can be described as externalization or combination by the SECI model.
Such platforms have revolutionized the way developers work, introducing new channels to share knowledge in the form of pull requests, issues and wikis. 
It is unclear how these channels capture and share knowledge.
In this research, our goal is to analyze these communication channels in GitHub.
First, using the SECI model, we are able to map how knowledge is shared through the communication channels.
Then in a large-scale  topology analysis  of seven library package projects (i.e., involving over 70 thousand projects), we extracted insights of the different communication channels within GitHub. 
Using two research questions, we explored the evolution of the channels and adoption of channels by both popular and unpopular library package projects. 
Results show that (i) contemporary GitHub Projects tend to adopt multiple communication channels, (ii) communication channels change over time and (iii) communication channels are used to both capture new knowledge (i.e.,  externalization) and  updating existing knowledge (i.e., combination).


## Contents
* `dataset` - a directory of data in a `CSV` format.
* `figure` - figures of the resulted TDA.
* `script` - python code run on jupyter notebook.
* `README.md` - this file.

## How to run
1. Clone this repository into your userhome folder in the system :
   ```
   git clone https://github.com/NAIST-SE/TDA_Communication_Channels.git
   ```
   output: `/Users/<yourusername>/TDA_Communication_Channels/`
   
2. To get the raw dataset, download the source file from [libraries.io](https://zenodo.org/record/1196312/files/Libraries.io-open-data-1.2.0.tar.gz). Extract the file.

3. Copy file `projects_with_repository_fields-1.2.0-2018-03-12.csv` from the extracted directory `Libraries.io-open-data-1.2.0`, paste it into directory `TDA_Communication_Channels/dataset/`.

4. Open `Jupyter Notebook`, run script `TDA_Communication_Channels/scripts/preprocessing_libraries_io.ipynb`. The results (csv files) will be created in directory `dataset`.

5. Use [Knotter](https://github.com/rosinality/knotter) tool to generate the TDA from the results. The tool can be downloaded [here](https://pypi.org/project/knotter/).

## Documentations
The information captured from the package of `Projects with related Repository fields`:

| No | Attributes                                    | Related Channels         | Description
|---:|-----------------------------------------------|--------------------------|----------------------------
|  1 | Repository Fork?                              | Fork                     | Project is a copy of another project
|  2 | Repository Forks Count                        | # of Forks               | Measure of other projects related this project
|  3 | Repository Issues enabled?                    | Issue Tracker            | Project explicitly states issues in an Issue Tracking System
|  4 | Repository Wiki enabled?                      | Wiki                     | Knowledge is shared on a Wiki
|  5 | Repository Pages enabled?                     | GitHub Pages             | Knowledge is shared as a web page
|  6 | Repository Open Issues Count                  | # of Open Issues         | Measure of developer workloads
|  7 | Repository Readme filename                    | Readme                   | Knowledge is put on the GitHub front page
|  8 | Repository Changelog filename                 | Changelog                | Documents all changes to the source code
|  9 | Repository Contributing guidelines filename   | Contributing Guidelines  | Knowledge is put for newcomers to the project
| 10 | Repository License filename                   | License                  | Project documents knowledge of licensing
| 11 | Repository Code of Conduct filename           | Code of Conduct          | Project documents Code of Conduct regulations
| 12 | Repository Security Threat Model filename     | Security Threat Model    | Projects documents security regulations
| 13 | Repository Security Audit filename            | Security Audit           | Projects conducts security audits

## Authors
* Jirateep Tantisuwankul - Kasetsart University, Thailand
* [Yusuf Sulistyo Nugroho](https://yusufsn.github.io/) - Nara Institute of Science and Technology, Japan
* [Raula Gaikovina Kula](https://raux.github.io/) - Nara Institute of Science and Technology, Japan
* [Hideaki Hata](https://hideakihata.github.io/) - Nara Institute of Science and Technology, Japan
* Arnon Rungsawang - Kasetsart University, Thailand
* Pattara Leelaprute - Kasetsart University, Thailand
* Kenichi Matsumoto - Nara Institute of Science and Technology, Japan

## Publication
Available at: https://doi.org/10.1016/j.jss.2019.110416

Our dataset are published on the public domain, so that anyone may freely build upon, enhance and reuse the dataset for any purposes without restriction under copyright or database law.
