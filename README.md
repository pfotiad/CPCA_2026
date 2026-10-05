# CPCA_2026

The attached Jupyter Notebook (**CPCA_framework.ipynb**) contains code that will apply a *Complex Principal Component Analysis* framework to decompose fMRI time-series into a series of spatiotemporal patterns of propagation. From these patterns, we identify the *N* dominant ones (here, *N* = 4), and further characterize their properties. We specifically focus on their propagation duration as well as regional power. 

This code represents a minimal framework of the code used for the publication: **Fotiadis P, Jang H, Dai R, Li D, Cofré R, Timmermann C, Nutt DJ, Carhart-Harris RL, Mashour GA, Hudetz AG, Huang Z. "Reorganization of Human Brain Waves Across Diverse States of Consciousness" Submitted (2026)**, and has been adapted to run for any given fMRI matrix of size: time-points x brain regions. It assumes that the fMRI time-series have already been preprocessed and denoised. fMRI parameters specific to the acquisition (such as repetition time) can be specified under "Inputs and Parameters" below. 

Other relevant publications that might be useful to the interested reader -- which have also helped shape the code below -- are:
1. Bolt, T., Nomi, J.S., Bzdok, D. et al. A parsimonious description of global functional brain organization in three spatiotemporal patterns. Nat Neurosci 25, 1093–1103 (2022) -> github code: https://github.com/tsb46/BOLD_WAVES/blob/master/figures.ipynb
2. Byeon, K., Park, H., Park, S. et al. Developmental variations in recurrent spatiotemporal brain propagations from childhood to adulthood. Nat Commun 17, 1012 (2026) -> github code: https://github.com/HumanBrainED/Neurodev-CPCA/blob/main/scripts/cpca.py
