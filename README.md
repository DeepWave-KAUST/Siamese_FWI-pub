![LOGO](https://github.com/DeepWave-KAUST/Siamese_FWI/blob/main/asset/Fig11.png)

Official reproducible material for **SiameseFWI: A Deep Learning Network for Enhanced Full Waveform Inversion - Omar M. Saad, Randy Harsuko, and Tariq Alkhalifah**


# Project structure
This repository is organized as follows:

* :open_file_folder: **asset**: folder containing logo;
* :open_file_folder: **data**: folder containing Marmousi2 and overthrust models data;
* :open_file_folder: **utils**: set of common function to run FWI;
* :open_file_folder: **Model**: containing Siamese network;
* :open_file_folder: **results**: containing the reconstructed velocity model using SiameseFWI;
* :open_file_folder: **deepwave-old**: containing the old version of the DeepWave package.
  

## Notebooks
The following notebooks are provided:

- :orange_book: ``SiameseFWI_Marmousi.ipynb``: the main notebook performing the SiameseFWI for Marmousi model;
- :orange_book: ``SiameseFWI_overethrust.ipynb``: the main notebook performing the SiameseFWI for overthrust model;
- :orange_book: ``SiameseFWI_bad_initial_Overthurst.ipynb``: the main notebook performing the SiameseFWI for overthrust model; bad initial model;


## Getting started :space_invader: :robot:
- To ensure the reproducibility of the results, we suggest using the `FWIGAN.yml` file when creating an environment.
- Please install deepwave 0.0.8 version, which is used in this project.


Run:
```
./install_env.sh
```
It will take some time, but if you see the word `Done!` on your terminal you are ready to go. 

Remember to always activate the environment by typing:
```
conda activate FWIGAN
```
To install the old version of the DeepWave package, navigate to the "deepwave-old" folder, and run:
```
cd ./deepwave-old/
python setup.py install
```

**Disclaimer:** All experiments have been carried on a Intel(R) Xeon(R) CPU @ 2.10GHz equipped with a single NVIDIA GEForce RTX 3090 GPU. Different environment configurations may be required for different combinations of workstation and GPU.

## Cite us 
```bibtex
@article{saad2024siamesefwi,
  title={SiameseFWI: A deep learning network for enhanced full waveform inversion},
  author={Saad, Omar M and Harsuko, Randy and Alkhalifah, Tariq},
  journal={Journal of Geophysical Research: Machine Learning and Computation},
  volume={1},
  number={3},
  pages={e2024JH000227},
  year={2024},
  doi={https://doi.org/10.1029/2024JH000227},
  publisher={Wiley Online Library}
}
