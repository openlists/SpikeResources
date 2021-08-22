# SpikeResources

This is a collection of tooling and resources for spikes - including spike sorting and analyses of single- and multi-unit data.

## Table of Contents

- [Spike Sorting](#spike-sorting)
- [Spike Analyses](#spike-analyses)

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
- [spikeextractors](https://github.com/SpikeInterface/spikeextractors)
- [spiketoolkit](https://github.com/SpikeInterface/spiketoolkit)
- [spikesorters](https://github.com/SpikeInterface/spikesorters)
- [spikecomparison](https://github.com/SpikeInterface/spikecomparison)
- [spikewidgets](https://github.com/SpikeInterface/spikewidgets)
- [spikemetrics](https://github.com/SpikeInterface/spikemetrics)

SpikeInterface includes the access to multiple algorithms that can be used through the tool, including this
[list of spike sorters](https://spikeinterface.readthedocs.io/en/latest/install_sorters.html).

#### Spike Forrest

[SpikeForrest](https://spikeforest.flatironinstitute.org/) is a project that systematically compares multiple spike sorting algorithms.

### Spike Sorters

Spike sorters used on human single-neuron data:
- [waveclus](https://github.com/csn-le/wave_clus)
- [combinato](https://github.com/jniediek/combinato)
- [klusta](https://github.com/kwikteam/klusta)
- [OSort](https://www.urut.ch/new/serendipity/index.php?/pages/osort.html)

Spike sorters used on high density / animal recordings:
- [kilosort2](https://github.com/MouseLand/Kilosort)

### Quality Control

The following:
- A [quality metrics guide](https://allensdk.readthedocs.io/en/latest/_static/examples/nb/ecephys_quality_metrics.html) from the Allen institute
- Notes on [spike sorting metrics](https://edmerix.github.io/SpikeSorting/) from [Ed Merricks](https://edmerix.github.io/)
- [UMS2K](https://github.com/danamics/UMS2K)

## Spike Analyses

General Tools:
- [Spykes](https://github.com/KordingLab/spykes)
- [buzzcode](https://github.com/buzsakilab/buzcode/tree/master/analysis/spikes)
- [elephant](https://github.com/NeuralEnsemble/elephant), which uses [neo](https://github.com/NeuralEnsemble/python-neo)
- [Phy](https://phy.readthedocs.io/en/latest/) is a Python tool providing a graphical interface for visualization and manual curation of large-scale electrophysiology data.

Individual Analyses / Paper Code:
- A [place cell tutorial](https://github.com/PeyracheLab/Tutorial_HDPlaceCells_Analysis)
- [Replay trajectory classification](https://github.com/Eden-Kramer-Lab/replay_trajectory_classification) code
- Code for [ictal recruitment](https://github.com/edmerix/Merricks-et-al-JNeurosci-2021)
- [Code](​https://github.com/GiocomoLab) from the [Giocomo Lab](https://giocomolab.weebly.com/)
