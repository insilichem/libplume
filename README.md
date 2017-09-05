# Plume Suite

Python Layer for Unified Modular Molecular Modeling.

It's composed of several independent graphical interfaces and commands for UCSF Chimera.


- **Calculation setup**

    - **Plume MD**: Setup MD calculations with OpenMM and ommprotocol

    - **Cauchian**: QM and QM/MM calculations setup

- **Visualization**

    - **PlumeView** (formerly GAUDIView): Lighweight visualization of results coming from docking, conformational search or multiobjective optimization

    - **PlumeViewGL (provisional name)**: Experimental web interface to depict molecules, docking solutions and relational mapping of residues

    - **OrbiTraj**: A subtle modification to UCSF Chimera's MD Movie extension to allow the visualization of volumetric data along a molecular trajectory

- **Analysis**

    - **NCIPlot GUI**: Straightforward interface to setup calculations for NCIPlot and visualize them

    - **NormalModes**: Perform Normal Modes Analysis and view them directly on-screen

    - **PLIPGui**: Depict protein-ligand interactions, as calculated with PLIP

    - **PoPMuSiCGUI**: Depict and apply the predictions made by PoPMuSiC calculations

    - **PropKaGUI**: Analyze and depict the expected pKa values of protein residues with PropKa 3.1

    - **SubAlign**: Align two, potentially different, molecules based on partial matches of substructures

# Installation

1 - If you don't have Chimera installed, download the [latest stable copy](http://www.cgl.ucsf.edu/chimera/download.html) and install it with:

    chmod +x chimera-*.bin && ./chimera-*.bin

2 - Create a new directory anywhere to host the GaudiView installation files. For example:
    
    mkdir -p ~/insilichem/plume  # any name is OK

3 - Open a new Chimera instance and click on `Favorites> Add to Favorites/Toolbar`. In this dialog, add the path of the directory you created in step 2 and click save.

4 - Download the [requirements.txt](requirements.txt) file and run:

    pip install --follow-dependency-links -U -t <~/insilichem/plume> -r <path/to/downloads/requirements.txt> 