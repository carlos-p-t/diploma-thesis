# Evaluating the Significance of Outdoor Advertising Utilizing Computer Vision

*Seminar 2 for Diploma Thesis*

*Carlos Andres Pizarroso Troncoso*

Welcome to my Master's Degree diploma thesis repository.

Please consider reading this before navigating through this repository, to understand the directories and the files within them.

## About the Seminar 2 Course requirements

Following the instructions from the [Seminar 2](https://dai.fmph.uniba.sk/w/Course:Project_Seminar_2/sk) course, this repository contains the following:

1) A presentation of the results of the Diploma Thesis for the Seminar 2 course (both a Power Point presentation and a PDF version of it).

2) A sample of the Diploma Thesis with the minimum of 15 pages in LaTeX including the front pages, abstract (in both languages), a list of the literature used in a PDF version (LaTeX files also included).

3) Samples of the implementation of the project with visual results in the form of Jupyter Notebooks.

4) Electronic samples studied for developing this part of the project.

## Brief description of the Project and the current development

**Objective:** To develop an automated system which evaluates road advertisement significance.

**Development:** In two phases: object detector development, classification system development.

For the **_Seminar 1_** course, a first attempt to train an object detector was made by merging 2 datasets (a larger one and a smaller one) achieving initial results.

For the **_Seminar 2_** course, after analyzing previous results, a different training method was tested: Training an object detector on the largest dataset first, and then fine-tune the resulting model in the smaller dataset, achieving significantly better results.

Additionally, we introduce our current work with the classification system (*under development*).


## How to navigate through this repository?

Below, a short description of the directories and main files of the repository:

The [Diploma LaTeX Files/src](https://github.com/carlos-p-t/diploma-thesis/tree/main/Diploma%20LaTeX%20Files/src) directory contains the Diploma Thesis LaTeX documents.

The [Framework](https://github.com/carlos-p-t/diploma-thesis/tree/main/Framework) directory contains the parts of the object detector system developed. It contains 3 subdirectories which are:

- [Data Subset Creator](https://github.com/carlos-p-t/diploma-thesis/tree/main/Framework/Data%20Subset%20Creator): Includes the notebook which extracted a subset of images from the larges dataset. The additional text files are the file names saved from this extraction. More details are included in the notebook itself.

- [Object Detector Training](https://github.com/carlos-p-t/diploma-thesis/tree/main/Framework/Object%20Detector%20Training): It contains two notebooks which show how the base training process was developed. It also includes the YAML file used for training the object detector.

- [Fine Tuning](https://github.com/carlos-p-t/diploma-thesis/tree/main/Framework/Fine%20Tuning): Includes two notebooks (1 per base model trained) and the respective YAML file used for fine tuning the object detector from the previous step.

The [Results](https://github.com/carlos-p-t/diploma-thesis/tree/main/Results) directory contains the notebook where the best models were tested on images and it is possible to see the capability of the object detector to detect billboards. Additionally, the best two models (after fine tuning) are uploaded in case someone wants to verify on custom dataset.

The [Studied Papers](https://github.com/carlos-p-t/diploma-thesis/tree/main/Studied%20Papers) include the electronic versions of the articles studied to develop this part of the project. They are also included properly in the Thesis Draft document.

The main documents included in this repository are:

* [Diploma Draft](https://github.com/carlos-p-t/diploma-thesis/blob/main/Diploma_draft.pdf): The LaTeX PDF version of the thesis progress, as requested by the requirements.

* The [presentation](https://github.com/carlos-p-t/diploma-thesis/blob/main/Evaluating%20the%20significance%20of%20outdoor%20advertising%20utilizing%20computer%20vision%20II.pptx) of the results achieved for this course, the [PDF](https://github.com/carlos-p-t/diploma-thesis/blob/main/Evaluating%20the%20significance%20of%20outdoor%20advertising%20utilizing%20computer%20vision%20II.pdf) version of this file is included for visualization purposes.

More details about the datasets, procedures, methodologies, and the results are explained in the Diploma Draft file.