## Repo for mp attn head issue

1 - Currenty relies on IMDB dataset, a subset is included with the clone but in case you need full dataset: (will switch to fake dataset shortly):

```
wget http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz 
tar -xf aclImdb_v1.tar.gz

```
2 - If needed - "pip install transformers" to install Hugging Face. 

3 - (optional) - modify the active policy and/or add new dataclass in the code (fsdp_mp.py) to adjust mixed precision params.
<img width="878" alt="mp_policy_control" src="https://user-images.githubusercontent.com/46302957/163057425-4a2bc941-bbd1-485a-a325-85d2deb4454b.png">



4 - Run with:
```
python fsdp_mp.py
```
