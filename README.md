<h1 align="center">
	Open Data Kazakhstan
<br />
	Docs for data engineers
</h1>

## Table of content

* [English version](#english-version)
  * [Getting started](#getting-started)
  * [Submitting an idea](#submitting-an-idea)
  * [Create a new dataset](#create-a-new-dataset)
  * [Contributing to an existing dataset](#contributing-to-an-existing-dataset)
  * [Datasets](#datasets)
    * [Metadata specification](#metadata-specification)
    * [Data format](#data-format)
    * [Scripts](#scripts)
    * [Data pipelines](#data-pipelines)
* Russian version
  * TODO
* Kazakh version
  * TODO
  
# English version

## Getting started

This is an open-source project fully hosted on GitHub. All contributions are welcome, whether it's a bug report, data engineering or documentation. Below you can find some details about different contributions to this project.

### Submitting an idea

Ideas for datasets can be submitted in [this issue tracker](https://github.com/open-data-kazakhstan/ideas/issues). Please, provide as much details as possible so that other people can easily understand the idea. Before creating an issue for your idea, make sure it doesn't exist already.

### Create a new dataset

When you start working on a new dataset, normally you wouldn't have an existing repository. In that case, you can create one with your own account on Github and transfer it to our organization. 

### Contributing to an existing dataset

If you found an issue/bug in an existing dataset repository, you can simply open a pull request and assign one of the members of this organization as a reviewer. Once it is reviewed and approved, we make sure it is merged into the main branch.

You can also create an issue for each dataset. Simply open a new issue in the relevant repository. Please, don't use `ideas` repository for issues in an existing dataset.

## Datasets

A single dataset can be placed in a repository, for instance, this is a population dataset: https://github.com/open-data-kazakhstan/population. It should have the following structure:

- `README.md` - a markdown based documentation for a given dataset. For example: https://github.com/open-data-kazakhstan/geo-boundaries-kz/blob/master/README.md
- `datapackage.json` - a metadata for a dataset. See [metadata specification](#metadata-specification) section for more details.
- `data/` - a directory where data files (e.g., `csv` files) are stored.
- `scripts/` - a directory where scripts to generate (e.g., process, transform etc.) data files are stored.
- `.github/workflows/` - a directory where we define [GitHub actions (data pipelines)](#data-pipelines).

### Metadata specification

We describe data using [frictionlessdata](https://frictionlessdata.io/) specification.

TODO: how to generate `datapackage.json`.

### Data format

We use CSV format for tabular data.

### Scripts

We use Python programming language by default and [Dataflows](https://github.com/datahq/dataflows) library.

### Data pipelines

TODO


