# Adaptive RL

- **ACSOS'25:** [6th IEEE International Conference on Autonomic Computing and Self-Organizing Systems](https://conf.researchr.org/home/acsos-2025) 

## Description
This repo contains the latex structure for the **Adaptive Reinforcement Learning: Algorithms and Implementation Strategies** paper.


## Structure 

* preamble: contains all package and command definitions. Everything should be set by now, but if something needs defining this is the place to do it (look inside to see the structure)
* bibfiles
    * local.bib: contains all local bib references i.e., references used for this paper specifically. Most references should be added here
    * bib folder: this folder contains many references used for multiple purposes, in particular the _compsci.bib_ file contains many references on software engineering, programming languages, and adaptive systems. Check here if the reference exists before adding it to the _local.bib_ file
	* THe bibfolder is usually added as a submodule to keep it consistent across repos. If you don't see the bib folder fetch it using: _git submodule update --init_
* Acronym.tex: contains all Acronyms used in the paper (look into the file for example of the definition). Acronyms are used with the \ac{ACRONYM} command
* Pointers to objects in the text (e.g., images, tables, code, sections, code-line, ....) are referenced using the fancyref package using the command \fref{} respectively starting with (img:, tab:, lst:, sec:, ln:, ....)


## Useful commands

* _\authorcomment[TYPE]{AUTHOR}{COMMENT}_ is used to leave annotation inlined with the text. Comments only appear in draft mode (the option in the documentclass in the _main.tex_ file) and are invisible otherwise. TYPE can be comment, missing, idea, note, and author.
* _\ie \eg \cf_ are used respectively for the abbreviations i.e., e.g., cf.
* listings are defined according to each specific language in the _preamble_ file and generate their own environment (e.g., _\ctxraits[....]{....}_ generates a contexts traits listing).
