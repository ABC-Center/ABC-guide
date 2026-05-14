# Quick-start to Python for Ecologists

Looking to implement AI/ML tools into your pipeline? Here's a quick-start guide with a collection of resources to help you get started.

## Getting Started

Let's start with a brief introduction to the basic coding scaffolding you'll need:

- **Programming languages** like R and Python can be run in [Integrated Development Environments (IDE)](ABC-Glossary.md#integrated-development-environment-ide) (e.g. **Rstudio** for R, and **Visual Studio Code** for Python).
    - [VSCode](https://code.visualstudio.com/) is a convenient, customizable Integrated Development Environment (IDE) for writing and editing code files in multiple languages, especially Python.
    - [RStudio](https://posit.co/products/open-source/rstudio) supports other languages as well, but is most commonly used for R.
- Many programmers find it useful to write scripts in “lab notebook”-style documents that integrate comments, code, and printing and plotting results (e.g., **R Markdown Notebooks** for R and **Jupyter Notebooks** for Python).
    - Notebooks provide space for exploration and testing, with more immediate feedback and nicely rendered documentation of design decisions alongside the code.
    - Jupyter Notebooks can be run and edited in [VSCode](https://code.visualstudio.com/docs/datascience/jupyter-notebooks).
- Programs and workflows can also be run ***on the command line***, specifically this is running a program through the **C**ommand **L**ine **I**nterface (CLI), a.k.a the **terminal**, **shell**, **console**, or "bash shell".
    - On Mac or Linux, open "Terminal" to get started.
    - On Windows, you'll need to install one first; we recommend [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/).
    - Some useful common commands can be found in the [Command Line Cheat Sheet](Command-Line-Cheat-Sheet.md).
    - To run your program through the CLI, save your code in a file with the correct file extension (e.g. `myfile.py`), and type into the command line something like
    ```console
    python myfile.py
    ```
- As your code evolves beyond ["Hello World!"](https://en.wikipedia.org/wiki/Hello,_world), it will likely require you to use some **packages** or **libraries**: code written by developers, which you can download and use to make your life easier. For Python packages, you’ll want to use an environment manager like **conda**.
    - Generally, you want to scope a single environment for a particular project or task.
    - Learn more about different Python environment managers on the [Virtual Environents Page](Virtual-Environments.md).
- For effective collaboration&mdash;with yourself and others&mdash;use **Git** (`git`) for version control and sync it to a remote, such as [GitHub](https://github.com/).
    - Learn more about the basics of, and motivations for, version control in [The Turing Way](https://book.the-turing-way.org/reproducible-research/vcs/).

Two great resources for lessons covering these topics: 

1. The [Missing Semester of Your CS Education](https://missing.csail.mit.edu/): a collection of computer science-themed lessons from MIT.

2. The [Software Carpentry Lessons](https://software-carpentry.org/lessons/): hands-on, guided introductions to the topics introduced above. Each of the Core Software Carpentry lessons is described and linked to below.

### Software Carpentries Lessons

!!! note
    You can work through these lessons on your own or check The Carpentries site for [upcoming workshops](https://software-carpentry.org/workshops/workshops-upcoming/) being offered virtually or at a location near you.

#### Working on the Command Line

Lesson: [The Unix Shell](https://swcarpentry.github.io/shell-novice/)

Work through each of the episodes in this lesson to gain a familiarity with Unix-based operating system basics. This lesson will prepare you for navigating the shell, i.e., working from the command line. We recommend you complete this before the GitHub lesson, since the *Git* lesson uses the command line.

#### Introduction to GitHub

Lesson: [Version Control with Git](https://swcarpentry.github.io/git-novice/)

This lesson introduces users to local version control with `git` through the command line, then builds to interacting with the remote (e.g., <https://github.com>). It provides a comparison of tools and features introduced in the command line with their analogous UI (user interface) options in the remote (online). It also covers some common conventions and includes discussions of open science (see also [The Turing Way's discussion](https://book.the-turing-way.org/reproducible-research/open/)) and some core repository files, such as `.gitignore`, license, and citation files (also covered in our [GitHub Repo Guide](Github-Repo-Guide.md)). 

For those using R, this lesson includes a supplemental section on [using Git from RStudio](https://swcarpentry.github.io/git-novice/14-supplemental-rstudio.html). VSCode also has a [Git integration](https://code.visualstudio.com/docs/sourcecontrol/github).

!!! tip "Pro tip"
    Follow the [GitHub Workflow Guide](The-GitHub-Workflow.md) to improve collaboration and help avoid conflicts. [GitHub Projects](Guide-to-GitHub-Projects.md) are also a particularly powerful tool for collaborative project management.

#### Basic Python

Many machine learning algorithms and workflows are run using Python. If you're not familiar with Python, there are many resources to help you gain familiarity. Below are two Carpentries lessons to get you started:

- [Programming with Python](http://swcarpentry.github.io/python-novice-inflammation)
- [Plotting and Programming in Python](http://swcarpentry.github.io/python-novice-gapminder)

### Introduction to Data Analysis with Python

This [data workshop training](https://youtu.be/71Ww42ddz9s) was first presented at the Imagomics All-Hands in 2024. It runs through an initial analysis of a simplified dataset, filling in a [dataset card](HF_DatasetCard_Template_mkdocs.md) as the data is explored, cleaned, and prepared for training. Notebooks and more information can be found in the [data workshop repo](https://github.com/Imageomics/data-workshop-AH-2024). To complete the training, follow the below instructions.

#### Key Packages

The key packages used in this workshop are described below, organized by their use-cases.

- Data wrangling: `pandas` (DataFrames, the data structure), `datasets` (for accessing the data from Hugging Face).
- Notebooks (where the work gets done): `jupyterlab`, `ipywidgets` .
    - The notebooks can be run in VSCode or by launching Jupyter from the command line (as done in the tutorial itself).
- Image handling and visualizations: `pillow`, `seaborn`.
- Machine learning tools: `scikit-learn`, `opencv`.

#### Tutorial step-by-step instructions

1. Clone the [workshop repository](https://github.com/Imageomics/data-workshop-AH-2024) and follow instructions to set up your local environment.
2. Read the [Key Learning Objectives](https://github.com/Imageomics/data-workshop-AH-2024/#key-learning-objectives).
3. Read the [Story of the Workshop](https://github.com/Imageomics/data-workshop-AH-2024/#story-of-the-workshop).
4. Follow along with the [workshop lesson](https://youtu.be/71Ww42ddz9s).
5. Review extra notes in the [Further Reading](https://github.com/Imageomics/data-workshop-AH-2024/tree/main/further_reading) section, which contains pointers and links to other resources.

### Modeling Overview

For more on various training paradigms, see the [training paradigms section of the ABC Glossary](ABC-Glossary.md#training-paradigms).
The glossary also covers [models](ABC-Glossary.md#model-aiml-version) such as [transformers](ABC-Glossary.md#transformer), [CLIP](ABC-Glossary.md#contrastive-language-image-pre-training-clip), and [diffusion models](ABC-Glossary.md#diffusion-models).

For a more general discussion of Machine Learning topics, [IBM has a detailed guide](https://www.ibm.com/think/machine-learning#605511093).

#### General hands-on practice

- Introductory [PyTorch tutorials](https://pytorch.org/tutorials/beginner/basics/intro.html), which has a full PyTorch machine learning workflow example.
- A [GitHub Repo](https://github.com/davidbau/how-to-read-pytorch) on "How to Read Pytorch", which may help with some foundational concepts.
- A [Medium article](https://medium.com/fullstackai/how-to-train-an-object-detector-with-your-own-coco-dataset-in-pytorch-319e7090da5) on training an object detector with Pytorch, if you'd rather read about it first (be warned: there are large codeblocks included).
- [Climate Change AI](https://www.climatechange.ai/tutorials?) has a number of tutorials across a wide variety of topics and skill levels.

#### Camera traps

[Megadector](https://github.com/agentmorris/MegaDetector/), fine-tuned for your particular setup, is often the go-to when dealing with camera trap data. Check out this [YouTube video](https://www.youtube.com/watch?v=LUkQVARAVFI) by Siyu Yang to help you get started.

#### Bioacoustics

See the [OpenSoundScape tutorial](https://opensoundscape.org/en/stable/classifier_guide/guide.html) by Lauren Chronister, Tessa Rhinehart, Sam Lapp, and Santiago Ruiz Guzman, for a conceptual introduction to the classifier training workflow. This will prepare you dive into the [OpenSoundScape Documentation](https://opensoundscape.org/en/latest/) and build on the basic tutorials, expanding to your own data and use cases.

#### Are there more options, you ask?

In addition to the resources described on this page, you may also want to check out the following resources from the broader ABC Community:

- [Data Science & Computing Cheat Sheet](https://docs.google.com/document/d/1YbOYnDZpRu6Jo1mpfg8m_zGeyY34NGECyxk2rNkH5eo/edit?usp=sharing) compiled by Tessa Rhinehart, Lauren Chronister, and Sara Beery with resources from both the [Kitzes](https://kitzeslab.org) and [Beery](https://beerys.github.io/) Labs. Some content links back to or is described in this guide, but there are other tutorials and resources that are not covered here.

- [Ecological Modeling with AI and Python](https://ecoforecast.org/workshops/statistical-methods-seminar-series/#ai-python) tutorial by Sara Beery and Timm Haucke as part of the [Ecological Forecasting Initiative and the ESA Statistical Ecology Section Statistical Methods Seminar Series](https://ecoforecast.org/workshops/statistical-methods-seminar-series).
