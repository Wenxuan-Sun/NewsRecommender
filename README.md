# NewsRecommender

LSTUR  is a news recommendation approach capturing users' both long-term preferences and short-term interests. The core of LSTUR is a news encoder and a user encoder. In the news encoder, we learn representations of news from their titles. In user encoder, we propose to learn long-term user representations from the embeddings of their IDs. In addition, we propose to learn short-term user representations from their recently browsed news via GRU network. Besides, we propose two methods to combine long-term and short-term user representations. The first one is using the long-term user representation to initialize the hidden state of the GRU network in short-term user representation. The second one is concatenating both long- and short-term user representations as a unified user vector.

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

Remember to use Tensorflow1.15.2, otherwise there are some modules cannot be found. 