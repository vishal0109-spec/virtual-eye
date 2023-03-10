# Attention-Beam-Image-Captioning

We present a heuristic of beam search on top of the encoder-decoder based architecture that gives better quality captions on three benchmark datasets: Flickr8k, Flickr30k and MS COCO.

Beam search helps in finding the most optimal caption that can be generated by the model instead of greedily choosing the word with best score at each decoding step. Following shows how a beam width (k) of 3 helps in generating better captions:


## Dependencies

For dependencies related to this project, `environment.yml` and `requirements.txt` files have been provided.

To install the dependencies using conda: 

```bash
conda env create -f environment.yml
conda env list
```

## Training

Reference data folder and annotations json file for the downloaded dataset (MSCOCO, Flickr8k, Flickr30k) in `create_input_files.py` and run the python script to create the required dataset.

To train a model run `python train.py`.
All training hyper-parameters are mentioned in `train.py`.



