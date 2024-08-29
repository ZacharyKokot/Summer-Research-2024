# An Implementation and Analysis of a Shadow Tomography Procedure

## Overview

In this project, I aim to present an implementation of the shadow tomography procedure, as described by Huang, Kueng, and Preskill in their paper [Predicting Many Properties of a Quantum System from Very Few Measurements](https://arxiv.org/pdf/2002.08953) along with an analysis of its performance and a comparison to complete state tomography. 

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Contact](#contact)

## Features

- Main Jupyter Notebook
- IBM Quantum Platform Demo
- Supplementary Information
- Data

## Installation

### Prerequisites

* Python 3.12.xx
* A Jupyter Notebook environment.
* Pip Python package manager.
* All prerequisite packages are included in the requirements.txt file and can be installed using pip. This is explained in [Installation Steps](#installation-steps).

### Installation Steps

1. Clone this repository into the directory of your choice.
2. Open a terminal instance and navigate to the path of the contents of this repository.
3. Create a virtual environment using the command `python -m venv .venv`.
4. Run the command `.\.venv\Scripts\activate` to activate the virtual environment.
5. Run the command pip `install -r requirements.txt` to install the required packages into your new virtual environment.

## Usage

In your Jupyter Notebook environment open the repository folder and set your Python kernel to the virtual environment you created during installation. You can now run and modify the contents of the [ShadowTomography](ShadowTomography.ipynb) and [IBMQuantumDemo](IBMQuantumDemo.ipynb) files. 

### Main Notebook

This notebook starts with a overview of complete state tomograph with some theoretical background on state representation/reconstruction. Along with this an implementation of a complete state tomography algorithm is given including demonstrations on systems of 1, 2, and 3 qubits. Then an overview of shadow tomography is given followed by a step by step implementation, testing, and demonstration of each part of complete procedure. These sections explore the sample and computational complexity of the implementation as well as demonstrate the situations in which the shadow tomography procedure outperforms the complete state tomography procedure. 

### IBM Quantum Demo

This notebook isn't intended as an extensive demonstration of how to use the IBM Quantum Platform but rather as a quick introduction into submitting jobs and testing your circuits before running them on one of IBM's QPUs. Follow along with the cells to see how to submit a basic job through the IBM Quantum Platform and refer to the [IBM documentation](https://docs.quantum.ibm.com/) for further clarification if needed. 

### Supplementary Information

For some portions of the code I implemented rather complicated formulas which I believed required further explanation. These explanations are contained in the [Supplementary Information](<Supplementary Information/SupplementaryInfo.pdf>) file so refer here for further details.  This document was written in LaTeX and all source code is included along with the compiled PDF.

### Data

Over the course of this project I generated various data sets of measurements on simulated quantum processors. The generation of this data takes time so to cut down on the run time of the main Jupyter notebook I generated the data sets a single time and stored them in the [Data](Data/) directory. The cells which generate this data within the notebook have a special command in their first line, `%%skip`, which prevents the cell from running. If you wish to regenerate data comment out this command and run the cell after running all other cells (cells are not isolated and need the results of previous cells to function correctly.).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Zachary Kokot - [zachary.kokot@ucalgary.ca](mailto:zachary.kokot@ucalgary.ca)

Project Link: [https://github.com/ZacharyKokot/Summer-Research-2024](https://github.com/ZacharyKokot/Summer-Research-2024)
