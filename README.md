# Template for _datasheet for dataset_

This is a template for a [datasheet for dataset](https://arxiv.org/abs/1803.09010).

The template is [here](./datasheet-for-dataset-template.md).

## What is a datasheet for a dataset?

[Datasheets for datasets](https://arxiv.org/abs/1803.09010) were created to increase transparency
of datasets.

> [Datasheets for datasets] document [the dataset] motivation, composition, collection process,
> recommended uses, and so on. [They] have the potential to increase transparency and accountability
> within the machine learning community, mitigate unwanted biases in machine learning systems, facilitate
> greater reproducibility of machine learning results, and help researchers and practitioners select more
> appropriate datasets for their chosen tasks.

The problem it is trying to solve:

> Despite the importance of data to machine learning, there is no standardized process for
> documenting machine learning datasets. To address this gap, we propose _datasheets for datasets_.

The datasheet is not a passive, after-the-fact document. Dataset creators are expected to read the
questions in the _motivation_, _composition_, and _collection process_ sections **before** they start
collecting data for the dataset. The questions in these sections have considerations that, if not taken
into account before data is gathered, cannot be easily rectified later. Similarly, the dataset creators
are expected to read the questions in the _preprocesssing/cleaning/labeling_, before they preprocessing
the raw data.

## Why use a markdown file for the datasheet?

The short explanation: using a markdown file allows us to easily compare (diff) one version
of the datasheet with another version. 

The longer explanation:

Datasets should be under version control, in the same way we put the code under version
control. Once under version control, we can compare one version against the other.

It is easier to follow the changes in a dataset when its datasheet is distributed together
with the dataset. If the dataset is under source control, so should be its datasheet.

Whenever there is a new version of the dataset, we also need to update its description.
In other words, we need to update its datasheet.

The datasheet distributed with a version should be in a format that is easy to compare with
previous version, to allow us to quickly see what has been changed. Markdown is simple, text
format, making it ideal for that.
