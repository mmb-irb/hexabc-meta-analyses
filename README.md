[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mmb-irb/hexabc-meta-analyses/HEAD)
[![](https://img.shields.io/badge/Google%20Colab-Open-orange?logo=google-colab)](https://colab.research.google.com/github/mmb-irb/hexabc-meta-analyses/)

### hexABC Meta-Analyses

***

This repository contains a collection of Jupyter Notebooks demonstrating how to perform meta-analyses using the [hexABC](https://mmb.irbbarcelona.org/webdev3/hexABC) database: a FAIR-compliant resource of atomistic molecular dynamics simulations of naked DNA.

These notebooks showcase how to programmatically access and analyze large-scale DNA simulation data using the hexABC REST API, enabling advanced structural and statistical investigations across thousands of DNA sequences.

***

### Contents

  - **01_bimodality_analysis.ipynb**  
    Extracts base pair-step helical parameters and explores bimodal behavior at the tetrameric and hexameric levels.
  - **02_hbond_fraying_analysis.ipynb**  
    Identifies breathing/fraying events by analyzing hydrogen bond patterns across specific nucleotide subsequences.
  - **03_meta_trajectory_clustering.ipynb**  
    Builds meta-trajectories from recurring fragments (e.g., A–T base pairs) across all simulations and performs clustering to identify dominant conformations.

***

### REST API Access

All notebooks use the [hexABC REST API](https://mmb.irbbarcelona.org/webdev3/hexABC/rest) to retrieve simulation metadata, structural parameters, and trajectory fragments. The API supports fine-grained queries by project, frame range, and nucleotide region.

***

### Conda Installation and Launch

```console
git clone https://github.com/mmb-irb/hexabc-meta-analyses.git
conda env create -f conda_env/environment.yml
conda activate hexABC_DB
jupyter-notebook 01_bimodality_analysis.ipynb
```

***

## Copyright & Licensing
This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [IRB](https://www.irbbarcelona.org/).

* (c) 2025 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)

Licensed under the
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.


