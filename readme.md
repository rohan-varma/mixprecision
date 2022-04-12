## Repo for mp attn head issue

1 - Currenty relies on IMDB dataset (will switch to fake dataset shortly):

```
wget http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz 
tar -xf aclImdb_v1.tar.gz

```
2 - modfiy the bfSixteen dataclass in the code (fsdp_mp.py) to adjust mixed precision params.

3 - Run with:
```
python fsdp_mp.py
```
