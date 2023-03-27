# Conda Environment Installation Commands

## Spike Interface Environment

```
conda deactivate
conda create -p ./pip_spike_interface_env python=3.9 --yes
conda activate ./pip_spike_interface_env 

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
