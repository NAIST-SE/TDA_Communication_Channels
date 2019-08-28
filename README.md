# Replication Package: A Topological Analysis of Communication Channels for Knowledge Sharing in Contemporary GitHub Projects

[https://github.com/NAIST-SE/TDA_Communication_Channels](https://github.com/NAIST-SE/TDA_Communication_Channels)

This is a replication package for the paper **A Topological Analysis of Communication Channels for Knowledge Sharing in Contemporary GitHub Projects**.
This artifact is a repository consisting of (a) dataset including (i) 3 files related to RQ1 with the information of Repository Fork?, Repository Forks Count, Repository Issues enabled?, Repository Wiki enabled?, Repository Pages enabled?, Repository Open Issues Count, Repository Readme filename, Repository Changelog filename, Repository Contributing guidelines filename, Repository License filename, Repository Code of Conduct filename, Repository Security Threat Model filename, Repository Security Audit filename, Platform; 
(ii) 7 files related to RQ2 including the information of Repository Fork?, Repository Forks Count, Repository Issues enabled?, Repository Wiki enabled?, Repository Pages enabled?, Repository Open Issues Count, Repository Readme filename, Repository Changelog filename, Repository Contributing guidelines filename, Repository License filename, Repository Code of Conduct filename, Repository Security Threat Model filename, Repository Security Audit filename, Platform, Repository Stars Count;
(b) figure contains all figures of topological data analysis; and 
(c) script, python code used in the research.


## Abstract
With over 28 million developers, success of GitHub collaborative platform is highlighted through the abundance of communication channels among contemporary software projects. 
Knowledge is broken into two forms and its transfer (through communication channels) can be described as externalization or combination by the SECI model of knowledge transfer of an organization.
Over the years, such platforms have revolutionized the way developers work, introducing new channels to share knowledge in the form of pull requests, issues and wikis. 
It is unclear how these channels capture and share knowledge.
In this research, our goal is to analyze how communication channels share knowledge over projects.
First, using the SECI model, we are able to map how knowledge is transferred through the communication channels.
Then in a large-scale topology analysis of seven library package platforms, we extracted insights of how knowledge is shared by different library ecosystems within GitHub. 
Using topology data analysis, we show that (i) channels tend to evolve over time and (ii) library ecosystems consistently have channels to capture new knowledge (i.e., externalization).
Results from the study aid in understanding what channels are important sources of knowledge, also with insights into how projects can attract and sustain developer contributions.


## Contents
* `dataset` - a directory of data in a `CSV` format.
* `figure` - figures of the resulted TDA.
* `script` - python code run on jupyter notebook.
* `README.md` - this file

## How to run
1. Clone this repository into your userhome folder in the system :
   ```
   git clone https://github.com/NAIST-SE/TDA_Communication_Channels.git
   ```
   output: `/Users/<yourusername>/TDA_Communication_Channels/`
   
2. To get the raw data, download the source file from [libraries.io](https://zenodo.org/record/1196312/files/Libraries.io-open-data-1.2.0.tar.gz). Extract the file.

3. Copy file `projects_with_repository_fields-1.2.0-2018-03-12.csv` from the extracted directory `Libraries.io-open-data-1.2.0`, paste it into directory `TDA_Communication_Channels/dataset/`.

4. Open `Jupyter Notebook`, run script `TDA_Communication_Channels/scripts/preprocessing_libraries_io.ipynb`. The results (csv files) will be created in directory `dataset`.

5. Use [Knotter](https://github.com/rosinality/knotter) tool to generate the TDA from the results. The tool can be downloaded [here](https://pypi.org/project/knotter/).

## Authors
* Jirateep Tantisuwankul - Kasetsart University, Thailand
* [Yusuf Sulistyo Nugroho](https://yusufsn.github.io/) - Nara Institute of Science and Technology, Japan
* [Raula Gaikovina Kula](https://raux.github.io/) - Nara Institute of Science and Technology, Japan
* [Hideaki Hata](https://hideakihata.github.io/) - Nara Institute of Science and Technology, Japan
* Arnon Rungsawang - Kasetsart University, Thailand
* Pattara Leelaprute - Kasetsart University, Thailand
* Kenichi Matsumoto - Nara Institute of Science and Technology, Japan

Our dataset are published on the public domain, so that anyone may freely build upon, enhance and reuse the dataset for any purposes without restriction under copyright or database law.
