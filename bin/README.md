# Conda Environment Installation Commands

## Spike Interface Environment

```
conda deactivate
conda create -p ./spike_interface_env python=3.9 --yes
conda activate ./spike_interface_env 

# Installing Jupyter Notebook
conda install -c conda-forge notebook --yes
# Installing Spectral Connectivty
conda install -c edeno spectral_connectivity --yes

# Installing Spike Interface
pip install spikeinterface[full]==0.97.1
# Installing sorters
pip install mountainsort4==1.0.3
```

## Phy Environment

```
conda deactivate
conda create -p ./phy_env python=3.9 --yes
conda activate ./phy_env 

# Installing phy
pip install phy --pre --upgrade
```

## Spike Interface Environment with Pip from Conda
```
# https://github.com/SpikeInterface/spikeinterface 
conda create -p ./spike_interface python=3.9 --yes
conda activate ./spike_interface
./spike_interface/bin/pip install spikeinterface[full,widgets]
./spike_interface/bin/pip install mountainsort4==1.0.3

# Installing Spectral Connectivty
conda install -c edeno spectral_connectivity --yes

# Installing Jupyter Notebook
conda install -c conda-forge notebook --yes

# Installing Git Library to get root directory of repo
conda install -c conda-forge gitpython
# To use GPU for spectral connectivity
# conda install -c conda-forge cupy
conda install -c conda-forge cupy cudatoolkit=11.0

# To label inlines
/nancy/projects/extracellular_ephys_analysis/bin/s
pike_interface

./spike_interface/bin/pip install matplotlib-label-lines

# To look at videos
conda install -c conda-forge opencv

conda install -c conda-forge seaborn

```
