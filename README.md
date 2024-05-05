# distilvit

Fine-tune a Visual Encoder Decoder model for image captioning.

Resulting model is available on Hugging Face model hub at https://huggingface.co/mozilla/distilvit

The train script is inspired from https://ankur3107.github.io/blogs/the-illustrated-image-captioning-using-transformers/#references

To install, use your favorite tools or you can run this:

```
python -m venv .
bin/pip install -r requirements.txt
bin/pip install -e .
```

To train against all image & caption pairs (COCO, Flickr30k and TextCaps), make sure you have 2T of disk space, and run:

```
bin/train --dataset all
```

Once trained, you can try it out with the test script:

```
bin/python distilvit/infere.py
```
