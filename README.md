# Theta and alpha power across fast and slow timescales in cognitive control

[![Up to date](https://img.shields.io/github/last-commit/phuycke/alpha_theta_timescales)](https://img.shields.io/github/last-commit/phuycke/alpha_theta_timescales)
[![Follow me](https://img.shields.io/twitter/follow/PieterHuycke?style=social)](https://twitter.com/PieterHuycke)
[![DOI paper](https://img.shields.io/badge/Paper-https%3A%2F%2Fdoi.org%2F10.1111%2Fejn.15320-blue)](https://doi.org/10.1111/ejn.15320)
[![DOI data](https://img.shields.io/badge/Data-%20%20https%3A%2F%2Fdoi.org%2F10.5281%2Fzenodo.4659714-blue)](https://doi.org/10.5281/zenodo.4659714)

## Overview

This GitHub repository contains the code used for the analysis and plotting done in the paper titled "Theta and alpha power across fast and slow timescales in cognitive control" by Pieter Huycke, Pieter Verbeke, C. Nico Boehler and Tom Verguts. A preprint of this article is available on [BioRxiv.](https://doi.org/10.1101/2020.08.21.259341) The code available in this repository relies on the data collected for our study. This data is also open access, and can be found in this [Open Science Framework repository](https://osf.io/2q5eh/) when the article is published. 

## Organization

The scripts are organized following the order defined in [the paper](https://doi.org/10.1101/2020.08.21.259341).

- Software environment
    * A list of all the softwares used in the Anaconda environment, and their version at the moment of submission
- Experiment
    * Code
        - The experiment code itself. Note that ```main (only sub-01).py``` is a version that was used for the first subject. This version was too long, and hence we used a shorter version for the other 29 subjects (```main.py```).
    * Stimuli
        - The stimuli used in this experiment. Same stimuli as used in [Ruge and Wolfensteller (2010)](https://doi.org/10.1093/cercor/bhp228). 
- Data preparation
    * Behavioral
        - Behavioral data rejection (```clean.py```)
        - Definition of our descriptive statistics (```descriptives.py```)
    * EEG
        - Custom code written to preprocess our EEG data (```eeg_helper.py```)
        - The preprocessing pipeline as described in 'Data Recording and Initial Processing' (```initial_processing.py```)
        - List of subject-specific rejected channels and rejected ICA components (```set_cleaning_parameters.py```)
- Analysis
    * Ordered list of the analyses associated with the results described in the paper. The scripts are ordered so that their order corresponds with the order of the results described in the manuscript. In-script comments refer to the specific analysis done
- Plots
    * Folders describe the specific figure, file names describe what specific part of the plot is created

## Programming environment   

**Python 3 Anaconda environment files**
- [PsychoPy3 (experiment run)](https://github.com/phuycke/alpha_theta_timescales/blob/main/0.%20Software%20environment/psychopy.yml)
- [EEG analysis (MNE)](https://github.com/phuycke/alpha_theta_timescales/blob/main/0.%20Software%20environment/mne.yml)
- [Data shaping and plotting](https://github.com/phuycke/alpha_theta_timescales/blob/main/0.%20Software%20environment/analysis.yml)

Unsure how to use these files? We refer to the [Anaconda3 documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)

--- 

**R (v. 3.6.3 - "Holding the Windsock")**    
Extra packages needed:
- dplyr v. 1.02
- lme4 v. 1.1-26
- lmerTest v. 3.1-3

## Contact

Pieter Huycke (corresponding author)

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/06/ORCID_iD.svg/2048px-ORCID_iD.svg.png" alt="orcid logo" style="float:left;width:24px;height:24px;margin-right:5px"><a href="https://orcid.org/0000-0002-8156-4419">0000-0002-8156-4419</a>

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_cTJMGw0u-6pa22rOEAxiIXcaOaGp-_PXxw&usqp=CAU" alt="mail logo" style="float:left;width:24px;height:24px;margin-right:5px"><a href="mailto:pieter.huycke@hotmail.com?Subject=EJN%20Paper%202021">Mail me concerning this paper</a>

---

Tom Verguts (principle investigator)

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/06/ORCID_iD.svg/2048px-ORCID_iD.svg.png" alt="orcid logo" style="float:left;width:24px;height:24px;margin-right:5px"><a href="https://orcid.org/0000-0002-7783-4754">0000-0002-7783-4754</a>

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_cTJMGw0u-6pa22rOEAxiIXcaOaGp-_PXxw&usqp=CAU" alt="mail logo" style="float:left;width:24px;height:24px;margin-right:5px"><a href="mailto:Tom.Verguts@UGent.be?Subject=EJN%20Paper%202021">Mail me concerning this paper</a>

---

<img src="https://cdn.pixabay.com/photo/2019/09/12/13/47/pictogram-4471660_1280.png" alt="website logo" style="float:left;width:24px;height:24px;margin-right:5px"><a href="https://www.cogcomneurosci.com/">Visit our lab website!</a>
