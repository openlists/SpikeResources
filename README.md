# SpikeResources

This is a collection of tooling and resources for spikes - including spike sorting and analyses of single- and multi-unit data.

To contribute a new link to a tool or resource, open an issue mentioning it, or a pull request with a link.

Note that single-unit datasets are listed in the 
[OpenData](https://github.com/openlists/ElectrophysiologyData) list.

## Table of Contents

- [Data Management](#data-management)
- [Spike Sorting](#spike-sorting)
- [Spike Analyses](#spike-analyses)

## Data Management

Single neuron data is recorded with multiple different amplifiers and recording systems from different companinies, often with different proprietary file formats. This section collects tools and resources related to data management for neural recordings and single-unit data. 

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

[Spike sorting](http://www.scholarpedia.org/article/Spike_sorting) is the process of the grouping spikes into clusters, that relate to putative individual neurons, for which there have been many proposed algorithms. The following resources relate specifically to spike sorting.

### Tutorials

Spike sorting tutorials:
- A [brief overview](https://www.simonsfoundation.org/flatiron/center-for-computational-mathematics/image-and-signal-processing/spikeforest/) of spike sorting from the Simons Foundation
- A [tutorial](https://www.cambridgeneurotech.com/webinars/spike-sorting) from cambridge neurotech
- A [tutorial](https://cbmm.mit.edu/learning-hub/tutorials/computational-tutorial/introduction-spike-sorting) from CBBM
- A [collection of tutorials](https://github.com/SpikeInterface/spiketutorials) from Spike Interface

### Spike Interface

[SpikeInterface](https://spikeinterface.readthedocs.io/en/latest/) is a collection of Python modules relating to spike sorting and associated processes.

The SpikeInterface ecosystem includes multiple related tool, including:
- [spikeextractors](https://github.com/SpikeInterface/spikeextractors) provides interfaces for data files
- [spiketoolkit](https://github.com/SpikeInterface/spiketoolkit) provides modules pre- & post-processing related to spike sorting
- [spikesorters](https://github.com/SpikeInterface/spikesorters) provides an interface for running supported spike sorters
- [spikecomparison](https://github.com/SpikeInterface/spikecomparison) provides tools for comparing and benchmarking sorting outputs
- [spikewidgets](https://github.com/SpikeInterface/spikewidgets) provides widgets for visualizations
- [spikemetrics](https://github.com/SpikeInterface/spikemetrics) provides metrics for spike sorting quality control

SpikeInterface includes the access to multiple algorithms that can be used through the tool, including this
[list of spike sorters](https://spikeinterface.readthedocs.io/en/latest/install_sorters.html).

### Spike Sorters

Spike sorters that can be used on microwires, such as in human single-neuron data:
- [waveclus](https://github.com/csn-le/wave_clus)
- [combinato](https://github.com/jniediek/combinato)
- [klusta](https://github.com/kwikteam/klusta)
- [OSort](https://www.urut.ch/new/serendipity/index.php?/pages/osort.html)
- [tridesclous](https://github.com/tridesclous/tridesclous)

Spike sorters that can be used on high density recordings, such as in animal recordings:
- [kilosort2](https://github.com/MouseLand/Kilosort)

### Comparisons & Quality Control

Spike sorting solutions can vary, and in general requires quality control procedures to ensure that sorting solution are robust and adequately reflect isolated units. Different spike sorters can give different solutions, and it may be useful to compare different spike sorters to each other. 

The following are systematic comparisons of different spike sorters:
- [SpikeForrest](https://spikeforest.flatironinstitute.org/) is a project that systematically compares multiple spike sorting algorithms.

The following are guides to quality control for spike sorting:
- A [quality metrics guide](https://allensdk.readthedocs.io/en/latest/_static/examples/nb/ecephys_quality_metrics.html) from the Allen institute
- Notes on [spike sorting metrics](https://edmerix.github.io/SpikeSorting/) from [Ed Merricks](https://edmerix.github.io/)

## Spike Analyses

The following collects tools and resources for analyzing (sorted) single neuron data. 

### General Toolboxes

General Tools:
- [Spykes](https://github.com/KordingLab/spykes) is a Python toolbox for spike data analysis & visualizations
- [elephant](https://github.com/NeuralEnsemble/elephant), which uses [neo](https://github.com/NeuralEnsemble/python-neo)
- [Phy](https://phy.readthedocs.io/en/latest/) is a Python tool providing a graphical interface for visualization and manual curation of large-scale electrophysiology data

### Simulations

The following are tools & utitilies for simulations of spiking data:
- [MEArec](https://github.com/alejoe91/MEArec) Python toolbox for simulating extra-cellular recordings on multi-unit arrays

### Individual Analyses

The following are dedicated tutorials for single-cell analyses:
- A [place cell tutorial](https://github.com/PeyracheLab/Tutorial_HDPlaceCells_Analysis)

The following are collection of metrics for particular analyses:
- A [collection of grid scores](https://github.com/klaragerlei/grid_score) for grid cell analysis

The following are code repositories for individual analyses / projects / papers:
- [Replay trajectory classification](https://github.com/Eden-Kramer-Lab/replay_trajectory_classification) code
- Code for [ictal recruitment](https://github.com/edmerix/Merricks-et-al-JNeurosci-2021) in human single-unit activity
- Matlab [code](https://github.com/NeuroLuke/KunzNeuron2021) for a project on egocentric boundary cells

The following are collections of code available from particular labs:
- [Code repositories](https://github.com/buzsakilab) (Matlab) from the [Buzsaki lab](https://buzsakilab.com/)
    - Includes the ['buzcode'](https://github.com/buzsakilab/buzcode) collection of analysis code
- [Code repositories](https://github.com/GiocomoLab) (mostly Matlab) from the [Giocomo Lab](https://giocomolab.weebly.com/)
- [Code repositories](https://github.com/LorenFrankLab) (mostly Python) from the [Frank Lab](https://franklab.ucsf.edu/)
- [Code repositories](https://github.com/MattNolanLab/) (mostly Python) from the [Nolan Lab](https://nolanlab.mvm.ed.ac.uk/)
    - Includes analysis code for [spatial ephys analysis](https://github.com/MattNolanLab/SpatialEphysAnalysis)
