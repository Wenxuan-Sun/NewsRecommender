# NewsRecommender

Something else

## Getting Started

To setup on your local machine:

1. Install Anaconda with Python >= 3.6. [Miniconda](https://conda.io/miniconda.html) is a quick way to get started.

2. Clone the repository

   ```bash
   git clone https://github.com/Wenxuan-Sun/NewsRecommender.git
   ```

3. create a conda environment

   ```bash
   cd NewsRecommender
   conda env create -f reco_gpu.yaml
   ```

4. Activate the conda environment and register it with Jupyter:

   ```bash
   conda activate reco_gpu*
   python -m ipykernel install --user --name reco_base --display-name "Python (reco)"
   ```

5. Start the Jupyter notebook server

   ```bash
   jupyter notebook
   ```

## Algorithm

See in lstur_MIND.ipynb