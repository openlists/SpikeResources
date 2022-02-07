# SpikeResources

This is a collection of tools & resources related to 'spikes' in neuroscience (action potentials recorded from individual neurons).

This list covers single-unit and multi-unit data, including data management, spike sorting, and available tools and analyses. 

To contribute a new link to a tool or resource, open an issue mentioning it, or a pull request with a link.

Note that single-unit datasets are listed in the 
[OpenData](https://github.com/openlists/ElectrophysiologyData) list.

## Table of Contents

- [Data Recording](#data-recording)
- [Data Management](#data-management)
- [Spike Sorting](#spike-sorting)
- [Spike Analyses](#spike-analyses)

## Data Recording

Single-unit data can be recorded with various different amplifiers and recording systems from different companies. 

This section lists companies that make recording systems for single-unit recordings.

### Recording Systems

- [BlackRock](https://blackrockneurotech.com/)
- [NeuraLynx](https://neuralynx.com/)
- [Ripple](https://rippleneuro.com/)
- [SpikeGadgets](https://spikegadgets.com/)
- [Intan](https://intantech.com/)
- [Open Ephys](https://open-ephys.org/)

## Data Management

Data from different recording system are often stored in proprietary file formats. 

This section collects tools and resources related to data management for neural recordings of single- an multi-unit data. 

### Neurodata Without Borders

[NWB](https://www.nwb.org/) is a standardized data schema that can be used to store single-unit data. 

Within the NWB ecosystem, there are the following associated tools:
- [pynwb](https://github.com/NeurodataWithoutBorders/pynwb), a Python interface for NWB files
- [matNWB](https://github.com/NeurodataWithoutBorders/matnwb), a Matlab interface for NWB files
- [NWB conversion tools](https://github.com/catalystneuro/nwb-conversion-tools) for converting and combining data from proprietary formats
- [NWB widgets](https://github.com/NeurodataWithoutBorders/nwb-jupyter-widgets) for visualizing data in NWB files

### Other Data Management Tools

Other tools related to data management for single-unit data include:
- [NEO](https://neuralensemble.org/neo/), a Python tool for reading neurophysiology file formats

## Spike Sorting

[Spike sorting](http://www.scholarpedia.org/article/Spike_sorting) is the process of the grouping spikes into clusters, that relate to putative individual neurons. There have been many proposed algorithms for spike sorting. This section lists tools and resources related to spike sorting.

### Tutorials

Spike sorting tutorials:
- A [brief overview](https://www.simonsfoundation.org/flatiron/center-for-computational-mathematics/image-and-signal-processing/spikeforest/) of spike sorting from the Simons Foundation
- A [collection of tutorials](https://github.com/SpikeInterface/spiketutorials) from Spike Interface
- A [tutorial](https://www.cambridgeneurotech.com/webinars/spike-sorting) from cambridge neurotech
- A [tutorial](https://cbmm.mit.edu/learning-hub/tutorials/computational-tutorial/introduction-spike-sorting) from CBBM
- A [brief lesson on spike sorting](https://github.com/BIPN145/SpikeSorting) from a class
- A [brief, standalone tutorial](https://github.com/michnard/SpikeSortingTutorial) on spike sorting 

### Spike Interface

[SpikeInterface](https://spikeinterface.readthedocs.io/en/latest/) is a Python module for performing spike sorting and associated processes.

SpikeInterface can be used to run multiple available spike-sorting algorithms, including this
[list of spike sorters](https://spikeinterface.readthedocs.io/en/latest/install_sorters.html).

SpikeInterface includes multiple sub-modules, including:
- `comparison` for comparing and benchmarking sorting outputs
- `extractors` for interfacing with data files
- `toolkit` for pre- & post-processing related to spike sorting
- `sorters` for running supported spike sorters
- `widgets` for using widgets for visualizations

### Spike Sorters

Spike sorters that can be used on single-channel / microwire recordings, such as in human data:
- [combinato](https://github.com/jniediek/combinato), in Python
- [klusta](https://github.com/kwikteam/klusta), in Python
- [tridesclous](https://github.com/tridesclous/tridesclous), in Python
- [waveclus](https://github.com/csn-le/wave_clus), in Matlab
- [OSort](https://www.urut.ch/new/serendipity/index.php?/pages/osort.html), in Matlab
- [HDsort](https://git.bsse.ethz.ch/hima_public/HDsort), in Matlab
- [MountainSort](https://github.com/flatironinstitute/mountainsort), in C++

Spike sorters that can be used on multi-channel / high density recordings, such as in animal data:
- [HerdingSpikes2](https://github.com/mhhennig/hs2), in Python
- [YASS](https://github.com/paninski-lab/yass), in Python
- [SpykingCircus](https://github.com/spyking-circus/spyking-circus), in Python
- [kilosort3](https://github.com/MouseLand/Kilosort), in Matlab
- [IronClust](https://github.com/flatironinstitute/ironclust), in Matlab

### Comparisons & Quality Control

Spike sorting solutions can vary, and in general requires quality control procedures to ensure that sorting solution are robust and adequately reflect isolated units. Different spike sorters can give different solutions, and it may be useful to compare different spike sorters to each other. 

The following are guides to quality control for spike sorting:
- A [quality metrics guide](https://allensdk.readthedocs.io/en/latest/_static/examples/nb/ecephys_quality_metrics.html) from the Allen institute
- Notes on [spike sorting metrics](https://edmerix.github.io/SpikeSorting/) from [Ed Merricks](https://edmerix.github.io/)

The following are systematic comparisons of different spike sorters:
- [SpikeForrest](https://spikeforest.flatironinstitute.org/) is a project that systematically compares multiple spike sorting algorithms.

## Spike Analyses

The following collects tools and resources for analyzing (sorted) single neuron data. 

### General Toolboxes

General Tools:
- [Spykes](https://github.com/KordingLab/spykes) is a Python toolbox for spike data analysis & visualizations
- [elephant](https://github.com/NeuralEnsemble/elephant), which uses [neo](https://github.com/NeuralEnsemble/python-neo)
- [Phy](https://phy.readthedocs.io/en/latest/) is a Python tool providing a graphical interface for visualization and manual curation of large-scale electrophysiology data
- [Brainstorm](https://neuroimage.usc.edu/brainstorm/), a general purpose, Matlab toolbox, has tools for processing 
[ephys data](https://neuroimage.usc.edu/brainstorm/e-phys/Introduction)

### Simulations

The following are tools and utilities for simulating spiking data:
- [MEArec](https://github.com/alejoe91/MEArec), a Python toolbox for simulating extra-cellular recordings on multi-unit arrays
- [PyRates](https://github.com/pyrates-neuroscience/PyRates), a Python framework for rate-based neural simulations
- [Brian2](https://brian2.readthedocs.io/en/stable/), a Python toolbox for simulating spiking neural networks

### Individual Analyses

The following are dedicated tutorials for single-cell analyses:
- A [place cell tutorial](https://github.com/PeyracheLab/Tutorial_HDPlaceCells_Analysis)

The following are tools and resources for particular analyses:
- A [collection of grid scores](https://github.com/klaragerlei/grid_score) for grid cell analysis

The following are code repositories for individual analyses / projects / papers:
- [Replay trajectory classification](https://github.com/Eden-Kramer-Lab/replay_trajectory_classification) code
- Code for [ictal recruitment](https://github.com/edmerix/Merricks-et-al-JNeurosci-2021) in human single-unit activity
- Matlab [code](https://github.com/NeuroLuke/KunzNeuron2021) for a project on egocentric boundary cells

The following are collections of available code from individual labs:
- [Code repositories](https://github.com/buzsakilab) (Matlab) from the [Buzsaki lab](https://buzsakilab.com/)
    - Includes the ['buzcode'](https://github.com/buzsakilab/buzcode) collection of analysis code
- [Code repositories](https://github.com/GiocomoLab) (mostly Matlab) from the [Giocomo Lab](https://giocomolab.weebly.com/)
- [Code repositories](https://github.com/LorenFrankLab) (mostly Python) from the [Frank Lab](https://franklab.ucsf.edu/)
- [Code repositories](https://github.com/MattNolanLab/) (mostly Python) from the [Nolan Lab](https://nolanlab.mvm.ed.ac.uk/)
    - Includes analysis code for [spatial ephys analysis](https://github.com/MattNolanLab/SpatialEphysAnalysis)
