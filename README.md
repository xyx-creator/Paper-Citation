# Download dataset & environment

wget -q -O arxiv.zip https://snap.stanford.edu/ogb/data/nodeproppred/arxiv.zip

wget -q -O titleabs.tsv https://snap.stanford.edu/ogb/data/misc/ogbn_arxiv/titleabs.tsv

put titleabs.tsv in arxiv/mapping

Create a virtual environment and download packages in Requirements.txt

# Code explanation

gat_ogbn_scibert.ipynb: embeddings are generated from SciBERT with text from ogbn

gat_ogbn_original.ipynb: ablation experiments where we use embeddings provided by OGBN-Arxiv

You may need to uncomment some code to generate scibert_titleabs_embeddings_with_id.pt ogbn_arxiv_link_data_scibert.pt ogbn_arxiv_link_data_ogb.pt