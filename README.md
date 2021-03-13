# brl_ocr

This repository contains a dataset of labeled and un-labeled images
which is an extension of [DSBI](https://github.com/yeluo1994/DSBI) and [AngelinaDataset](https://github.com/IlyaOvodov/AngelinaDataset).

The dataset will be used for creation of a Braille characters detector based on the [AngelinaReader](https://github.com/IlyaOvodov/AngelinaReader).
The current version of the detector is here: [zuevval/AngelinaReader](https://github.com/zuevval/AngelinaReader)

# Requirements
Git with Git LFS

To find out whether you have Git with LFS installed, run 

```git lfs --version```

# Usage
## Downloading data
To checkout the files:

```git clone --recursive https://github.com/braille-systems/brl_ocr.git```

## Working with labels
Labels for data are made with [labelme](https://github.com/wkentaro/labelme).
To view, add or edit them, install and run this tool (preferrably in a fresh pip environment):
```
python -m pip install labelme
labelme --config .labelmerc
```
Open the desired picture, e. g. `brl_ocr/data/labeled/books/golubina/IMG_2504.JPG`:

![braille book with rectangles painted around each letter](https://user-images.githubusercontent.com/23435506/111027233-fe394f80-83ff-11eb-9f53-6234c2090dc9.png)


