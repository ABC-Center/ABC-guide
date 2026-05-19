# ABC Glossary

This glossary is designed as a resource for members of the ABC Global Center from various backgrounds to familiarize themselves with key terms and concepts encountered in our work.

It includes concepts in biology, biodiversity, ecology, genetics, machine learning and artificial intelligence, computer science, and software engineering.

Definitions are not meant to be comprehensive. Ideally, they will be tailored to ABC's context.

It is meant to be a collaborative effort, so please [contribute](https://github.com/ABC-Center/ABC-guide/issues) terms you would like defined, definitions you know, or corrections for errors you notice!

## A

### Application Programming Interface (API)

### Autoencoder

## B

### Biodiversity

Biodiversity has the dictionary definition of the “variety of life on earth”. In practice, this word can be broad to the point of almost being useless (“sure fine, but the devil is in the details”). It is often used as a generic catch-all phrase for “nature” or “life” or even “wildlife” in common colloquial use, like “protect biodiversity”, even though none of these are quite the same thing.

Ecologists tend to think about biodiversity explicitly in terms of scales of organization. Probably the two most common ways of thinking about scale are spatial scale and levels of organization, which are sometimes correlated but are not the same thing.

**Spacial scales** and how to think about them:

- *Global* is the entire planet.
- *Continental*, think the Americas.
- *Regional*, think the East Coast of the US.
- [*Landscape*](#landscape): Approximately the scale at which spatial processes (such as dispersal and migration) operate for many charismatic plant and wildlife species. Note that landscape ecologists define landscape not as a spatial scale but as a field concerned with the operation of ecological processes across a heterogeneous backdrop.
- *Site*, as in one field site or study area (the term may also be applied to a particular sampling location within the study area). The sites themselves might differ vastly in terms of area–from $1m^2$ (or smaller) for things like experimental plots to tens of km (e.g., the Breeding Bird Survey’s “site” is ~40km long).

**Levels of organization**:

- [*Ecosystem*](#ecosystem): All of the organisms present along with their abiotic conditions. Focused on flows of energy or nutrients, or webs of interactions, between living members of a community and abiotic stocks. Ecosystem ecology has the most overlap with environmental science, and often thinks in box models or similar. Most overlap with climate modeling and climate science. Much canonical work was and is done in wetlands and aquatic systems.
- *Community*: The various populations of many species present at the same location and interacting with each other. Canonical topics are interactions (i.e., consumer-resource interactions, competition, mutualisms), and coexistence (e.g., why are there so many species?). This is what most outside the field think of when they think of “ecology” in general.
- [*Population*](#population): A single interacting group of organisms of a single species. Canonical topics include how populations are regulated (i.e., how their size is determined), what factors cause them to grow and shrink. Closely related to single-species conservation as trends in population size are often a quantity that is monitored and used to make conservation/management decisions.
- *Organismal*: At the scale of a single organism or below. Included in, but not a main focus of, ABC. Note that just because something is at this scale or smaller does not mean it’s organismal or sub-organismal biology&mdash;in the case of eDNA for example, the DNA is used as sign to indicate the presence of an organism, with questions and research usually conducted at the population or community level.

#### Biodiversity Science

This is not yet a discipline that is officially defined; it means different things to different people.

### Biology

The study of living things, things that reproduce themselves (including bacteria).

## C

### CARE Principles for Indigenous Data Governance

"People and purpose-oriented" to complement [FAIR Principles](#fair-data-principles).

**C**ollective Benefit

**A**uthority to Control

**R**esponsibility

**E**thics

For more information, see [CARE Principles for Indigenous Data Governance](https://www.gida-global.org/care).

### Checklist

- List of species that are known to occur in a region (e.g., birds of Vermont).
- List of species that were seen and not seen during a fixed survey.

### Contrastive Language-Image Pre-training (CLIP)

Contrastive language-image pretraining (CLIP) is a training objective that popularized the idea of training strong vision models from language supervision, rather than class supervision. ImageNet is the classic labeled image dataset: 1.2M images where each image is labeled with one class out of one thousand possible classes.

CLIP enables learning strong vision representations from image-caption pairs scraped on the internet.

CLIP also enables zero-shot image classification.

## D

### Decoder

### Diffusion Models

Diffusion models are a class of models used to generate images. They are the architecture for models like Stable Diffusion and DALL-E 3. They learn to reduce the noise in an image by just a little bit, conditioned on some text representation. Then, starting with pure random noise, you can iteratively apply a diffusion model to produce a new image.

### Dimensionality Reduction

Used in machine learning and data analysis to refer to a set of methods used to reduce the number of variables or features under consideration to a smaller subset with the greatest explanatory power without drastically reducing the accuracy of the model or analysis. The purpose is to exclude irrelevant, redundant, and noisy information, thereby improving computational complexity and model interpretability.

That is, it seeks to preserve the "most important" variables or features of the data based on some quantitative metric, such as variance, while removing "less important" variables or features. This is especially helpful when using high-dimensional data such as images or genomes.

Dimensionality reduction techniques can be subdivided into two main categories:

- [Feature Extraction](#feature-extraction)
- [Feature Selection](#feature-selection)

### Docker

## E

### Ecology

The study of ecosystems: how organisms interact with each other and their environments.

### Ecosystem

There are many definitions:

- A set of potentially interacting organisms within their natural environment (including both biotic and abiotic environment).
- Some people distinguish ecosystems as being more often described by process (e.g., nutrient cycling), compared to biodiversity.

### Encoder

### Endemic

- In general when a species is found in one area and nowhere else (e.g. how many species are found exclusively in one region).
- Weighted endemism is more commonly used now for mapping; it is the percent of the distribution of one (or many) species in a grid cell (or other defined area). It’s the basis for spatial conservation planning.

### Entomology

The study of insects.

### Epoch (in machine learning)

### Evolution

The change in proportion of genes or traits within a population over the course of generations (many disagreements about this definition).
Sometimes short and long time scales are distinguished:

- **Short term**: over a few generations, prevalence of a gene changes.
- **Long term**: new species with new morphologies, a.k.a. body parts emerge.

### Experiment (in machine learning)

## F

### FAIR Data Principles

**F**indable -- metadata and data easily found by both humans and machines

**A**ccessible -- clear indication of how to access data once it is found.

**I**nteroperable -- ability to integrate with other data and be used by various systems (applications and workflows).

**R**eusable -- clearly described so it is easily used by others.

For more information, see [FAIR principles](https://www.go-fair.org/fair-principles/).

### Feature

In machine learning and data science, a feature is a single measurable property or characteristic of the phenomenon under observation. With tabular data, a feature is a column in the dataset used by a model to make predictions. In genomics, a feature could be, for example, gene expression levels, the presence (or absence) of certain genetic variants (such as [SNPs](#single-nucleotide-polymorphism-snp), insertions and deletions (indels), and others), or epigenetic markers.

#### Feature Extraction

A set of [dimensionality reduction](#dimensionality-reduction) techniques used to map raw data to a smaller set of features. Example techniques include [PCA](#principal-component-analysis-pca), [MDS](#multidimensional-scaling-mds), [t-SNE](#t-distributed-stochastic-neighbor-embedding-t-sne), [autoencoders](#autoencoder), and Fourier or wavelet transforms.

The key difference from feature selection is that feature extraction generates a new set of features from the original dataset by projecting or mapping the data into a new feature space rather than selecting from existing features.

#### Feature Selection

A method to select a subset of relevant features for use in model construction.

The key difference from feature extraction is that feature selection does not generate new features but rather identifies the most meaningful existing features in a dataset by excluding redundant or irrelevant features. For example, in genomics, feature selection would involve selecting the most important gene(s) relevant to a certain phenotype among thousands of genes.

#### Feature Space

### Fit (AI/ML Version)

A model may be "fit" to a particular training set, in that it is optimized for that data and/or training objective. A well fit model will perform well on its training data, but&mdash;more importantly&mdash;it will be *generalizable* to new data under the same objective (e.g., classification of animals in images that it has not seen).

- A model is considered to be *overfit* if it is too highly specialized to its training data, e.g., the model may perform near perfectly on museum specimen images it saw in training, but it cannot recognize the same species when photographed on a different background without a ruler.
- Conversely, a model is *underfit* if it does not capture the underlying structure of even its training data and thus does not perform well on either its training or unseen data. From the previous example, the model wouldn't recognize species in any of the images.
- IBM has a [nice general summary of these concepts](https://www.ibm.com/think/topics/underfitting).

### Fitness (Ecology Version)

There are many definitions; one would be the number of offspring (that survive to reproduce) of an individual animal.
People often talk about how certain traits contribute to fitness, e.g., longer giraffe necks = more food, better survival = more chances to reproduce.

### Foundation Model

A “foundation model” is a term coined by Stanford researchers in 2021 to describe large models trained on very general data that can adapt to a wide range of downstream tasks. It is another phrase to describe the pre-train/fine-tune paradigm introduced by computer vision researchers in the late 2010s.

Typically, a foundation model:

- Has many, many parameters.
- Is pre-trained (normally in a self-supervised fashion) on a huge quantity of data at great cost.
- Can be adapted to many different tasks **with significantly less data**, either through prompting (language models), fine-tuning (smaller foundation models) or linear probing ([vision models](#vision-models)).

### Functional Diversity

The variety of different forms and functions in a community/assemblage. [Traits](#trait) (such as body mass, diet, morphological characteristics) are often proxies of organism's functions in the ecosystem (think, e.g., long and pointy beaks in birds might imply nectarivorous diet, therefore pollination), and we use traits of species to quantify functional diversity.

## G

### Genome-Wide Association Study (GWAS)

## H

### Hyperparameter Tuning

The process of selecting the best hyperparameters for a machine learning model by minimizing the [loss function](#loss-function). This can be done through [experiments](#experiment-in-machine-learning) or in some cases, using optimization techniques. Hyperparameters are parameters that are set by the researcher before training and are not learned during the training process. Some examples of common hyperparameters are [learning rate](#learning-rate), number of [epochs](#epoch-in-machine-learning), number of clusters (k) in [k-means clustering](#k-means-clustering), and many others.  

## I

### Imageomics

i-'mi-j**ə**-'**ō**-miks

A new scientific field in which computational (machine learning) tools built around biological knowledge bases are used by biologists to analyze image data in order to characterize patterns and gain insights into traits and relationships at individual, population and species scales—insights that then get incorporated into the algorithms that run the tools.

### Inference

#### Inference (Ecology Version)

- Often used in reference to the interpretations/conclusions that we derive from our results/data analysis.
**Examples**:
    - “How does this covariate affect whether or not a species is present?” e.g. “When there are at least 50 trees with a diameter over XYZ within a 200m radius of this spot, you have a 90% chance of finding a Cerulean Warbler there”
        - These sorts of covariate-presence associations are often used for species distribution modeling
- Debates: Many ecologists make the distinction between inference versus prediction. Inference is more about ‘inferring’ relationships between variables and linking to theory, and not about trying to predict to new situations etc.; the emphasis is more about interpretation compared to making predictions.

### Integrated Development Environment (IDE)

Software or application designed with features to aid in software development, such as code editing, build automation, and debugging. Common examples include [VSCode](https://code.visualstudio.com/) and [RStudio](https://posit.co/products/open-source/rstudio), both of which include version control/tracking, with added options for git-based tracking integration (e.g., through [GitHub](https://github.com/) or [GitLab](https://about.gitlab.com/)). Additional options include formatting settings, compilers, and plugins for various language options. VSCode is often used for Python development and Jupyter Notebooks, while RStudio is generally recommended for R Code and R Markdown Notebooks.

## J

## K

### Keystone Species

Its removal will cause large shift in the community (the list and abundance of species); there are a handful of great examples where this is real, but it’s not expected that every ecosystem has “a keystone species”.

### K-Means Clustering

## L

### Landscape

On the order of 10s-100s of kilometers of land.
Important because it’s the scale at which individual organisms do stuff, like disperse from where they were born to where they’ll eventually breed.

### Latent Space

### Learning Rate

### Loss Function

## M

### Machine Learning (ML)

Machine learning is a way to make predictions about new data based on old, seen data. Fitting a regression to $1$-D data in Excel is the most obvious example of “machine learning”. But you can imagine using many more input variables $(x_1, x_2, … x_n)$ and also predicting more output variables $(y_1, y_2, … y_n)$.

As your data gets more complex, you probably want to choose a “line of best fit” that is more complex than just a line. Unfortunately, while fitting lines is very easy (it’s a convex optimization problem), fitting more complicated stuff is harder.

Part of the field of machine learning is developing new methods to efficiently and effectively fit complicated functions to complicated data.

### Model (AI/ML Version)

1. A specific set of parameters (also known as weights; they are just lots of numbers) optimized through training. [meta-llama/Llama-2-7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat) is a set of weights for the Llama2 7B variant.
2. A family of weights: Llama2 is the name for all Llama2 models, including different sizes (7B, 13B, 70B) and base/instruction-tuned versions.
3. An architecture: a transformer model refers to the general class of models that use self-attention (discussed later).

### Model (Ecology Version)

- Sometimes used in reference to mathematical models that arise from theory and describe relationships among components of an ecosystem.
    - **Example**: predator-prey model of population dynamics.
- Sometimes used in reference to statistical models that describe relationships among variables, relationship between predictor/explanatory variables (for example, environment or climate measures) and response variables (for example, species richness, or presence).
    - **Example**: occupancy models statistically associate covariates with species presence.

### Multidimensional Scaling (MDS)

## N

### Neural Network

A neural network is a type of model (function) with near-unlimited complexity. Because of this complexity, neural networks need lots of data to effectively “learn”, but they can fit very complicated datasets (for example, OpenAI’s GPT models have “fit” the English language).

### Nucleotide

The fundamental building blocks of DNA and RNA. A nucleotide is composed of a base and a sugar-phosphate backbone.

Bases for DNA: adenine (A), guanine (G), cytosine (C), and thymine (T).

Bases for RNA: adenine (A), guanine (G), cytosine (C), and uracil (U).

Backbone sugar for RNA: ribose

Backbone sugar for DNA: deoxyribose (one less oxygen atom than ribose)

The bases A, G, and C are the same molecule for DNA and RNA. T and U are incorporated into their sequences differently due to the presence of substrate molecules accessible to DNA polymerase and RNA polymerase, which are the enzymes responsible for "manufacturing" the relevant sequences. DNA polymerase must use deoxyribonucleotides (dNTPs), and RNA polymerase must use ribonucleotide triphosphates (NTPs). Again, the difference is that there is one less oxygen atom in dNTPs vs NTPs. Cells have dATPs, dGTPs, dCTPs, and dTTPs for DNA polymerase to incorporate into a DNA sequence, but there are normally no dUTPs (and in cases where dUTPs are present and incorporated into DNA, "error correction" enzymes replace them using dTTPs). Likewise for RNA polymerase, ATP, GTP, CTP and UTP are available, but TTP is not. These substrates also serve other important purposes, such as how ATP (adenosine triphosphate) is used as a primary source of energy for many cellular processes.

A DNA or RNA molecule consists of a chain of the four relevant nucleotides in a sequence, where the order of A, G, C, and T in the DNA sequence determines the "blueprint" for the organism, and the order and length of A, G, C, and U in an RNA sequence determines the purpose and function of the RNA molecule, which can be a messenger RNA (mRNA) that encodes a protein, a microRNA (miRNA) which are short RNAs that help regulate gene expression by binding to other mRNAs, and many others.

## O

### Ontology

### Operational taxonomic units (OTU)

Usually used in place of [“species”](#species) to describe and group single-celled organisms (e.g., bacteria). An OTU can be defined using metrics like genetic distance.

## P

### Phenotype

### Phylogeny

A tree of life, depicts evolutionary relationships among species, usually within one taxonomic group (birds, mammals, etc.), often used to quantify phylogenetic diversity of an assemblage (another aspect of biodiversity).

### Population

Population is often used in reference to a set of interacting or potentially interbreeding individuals of a single species, e.g., “all the frogs in this series of 3 ponds near each other form a population. It’s a distinct population from the ones in the other ponds that are too far for the frogs to hop to”.

### Pre-training

### Principal Component Analysis (PCA)

## Q

## R

### Range Shift

Change in the places a species is found over time, e.g. due to changes in temperature, vegetation, weather, etc.

## S

### Self-supervised Learning

Self-supervised learning is very popular in both language and vision right now. I will explain the dominant self-supervised learning strategies in both modalities.

**Causal language modeling**: given a token sequence $T_1, T_2, T_3, … T_N$, learn to predict the next token $T_{N+1}$. All text on the internet can be used for this task, and each sequence of $N$ tokens makes $N-1$ training examples.

**Masked language modeling**: given a token sequence $T_1, T_2, MASK, T_4, … T_N$, learn to predict T_3. Again, all text on the internet can be used for this task because we can replace any token with $MASK$ to make a training example.

**Vision SSL**: Given an image $IMG$, apply some augmentation to $IMG$ like color shifts, rotation, distortion, blur, crop, etc to make $IMG’$. Then minimize the distance between $f(IMG)$ and $f(IMG’)$ while maximizing distance between $f(IMG)$ and all other images.

**Contrastive Language Image Pre-Training (CLIP)**: Given a large dataset of (image, text) pairs, learn two models: one for images $f_i(x)$, one for text $f_t(x)$. Minimize the distance between $f_i(image)$ and $f_t(text)$ for true (image, text) pairs and maximize the distance for random (image, text) pairs not found in the data.

Self-supervised learning is all about finding a trick that enables learning useful representations without doing large-scale labeling.

### Single Nucleotide Polymorphism (SNP)

A SNP (pronounced "snip") is a variation in the [nucleotide](#nucleotide) present at a single position in a DNA sequence among individuals in a species. For example, a SNP may be the replacement of a cytosine (C) by a thymine (T) at the same location in a stretch of DNA, where C is observed in a subset of individuals and T is observed in the others.

### Snakemake

### Species

- A simplistic and debated definition: A group of organisms that regularly reproduce with each other.
- There are *many* different ‘species concepts’ and it really depends on your study question. It has a lot of relevance for conservation as we are often concerned with identifying (and protecting) 'endangered species'.
- **Longstanding debates**:
    - The ‘biological’ species concept assumes that different species should not be able to interbreed. *However*, that’s not true for many species, especially plants and invertebrates, microbes. There are also ‘lumpers’ and ‘splitters’:
        - Lumpers tend to aggregate into fewer species.
        - Splitters more likely to formally define many species.
    - With molecular markers etc, now there are ‘operational taxonomic units’ where we don’t need a formally defined species.
    - Definitions are influenced by bias: different parts of the world have different amounts of described species, so better known areas (e.g., US and Europe) have inflated diversity relative to understudied areas.

### Species distribution model (SDM)

An [ecological model](#model-ecology-version) that predicts where and when a species will be present based on covariates in the environment.
Also known as ecological niche models ‘ENM’ as they attempt to capture the ‘niche’ of a species, a term debated for the entire history of ecology, generally it is acknowledges that SDMs capture some version of the ‘realized’ niche rather than the fundamental/potential niche.

### Subspecies

### Supervised Learning

As opposed to [unsupervised learning](#unsupervised-learning), supervised learning methods learn from labeled data. That is, it is trained using input data that is labeled with corresponding outputs, such as the input of an image and the output of a classification.

## T

### Taxa (s. taxon)

*Taxa* is the plural of *taxon*, which is a rank of hierarchical classification system of organisms, most commonly Domain, Kingdom, Phylum, Class, Order, Family, Genus, Species, each representing a decreasingly large group of organisms. A “mountain bluebird” (*Sialia currucoides*) is a taxon, “amphibians” (members of class *Amphibia*) are also a taxon.

### Taxonomy

### t-Distributed Stochastic Neighbor Embedding (t-SNE)

### Training Paradigms

- [**Supervised learning**](#supervised-learning): Given a large dataset of (input, output) pairs, learn to predict the output given the input.
- [**Unsupervised learning**](#unsupervised-learning): Given a large dataset of (input) examples, learn something about the structure of the data (clustering, dimension reduction, etc)
- [**Self-supervised learning**](#self-supervised-learning): Given a large dataset of (input) examples, learn useful representations that can then be leveraged to do well on a supervised task.

### Trait

A characteristic of an individual organism such as e.g., its body mass, diet, when it is active (nocturnal, diurnal), clutch size (number of eggs it lays), color of wings, wing span, beak shape, etc. Traits are only traits if they can be measured on an individual, though there is still some debate over it--for example, some ecologists consider ‘species range’ a trait, but because it cannot be measured on an individual, it is not actually a trait.

- A trait is “functional” if it plays some function (most trait do, though we cannot often map traits to functions yet).
- A trait can be a ‘response trait’ or an ‘effect trait’: response traits describe an organism’s response to the environment, while effect traits describe the impact of this organism on the ecosystem's functioning.

### Transfer Learning

### Transformer

A transformer is a model architecture based on self-attention and feed-forward neural networks. They operate on sequences and can predict sequences or labels. There are three main variants: encoder-only, decoder-only and encoder-decoder. I will provide some examples of famous transformers to illustrate their strengths, weaknesses, and differences.

*As a rule of thumb, a token is about 3/4 of a word.*

#### Transformer Examples

**BERT** is an encoder-only language model transformer. Given a sequence of tokens, it produces a dense vector representation for each token and a representation for the entire sequence.

- Small model; can be trained on academic budget in 3 days
- Used for sequence classification (is this sentence about animals or humans?) and token classification (predict the subsequence of tokens that is about animals).
- Does not work with long contexts; limited to 512 token-length sequences.
- Encoder-only: looks at the entire sequence at once. Cannot generate new text.

**Llama2** (from Meta/Facebook) is a (family of) decoder-only language model transformers. Given a sequence of tokens, it produces a dense vector representation for each token and can sample new tokens that continue the sequence.

- 7B, 13B and 70B variants. Cannot be trained on an academic budget. 7B and 13B can do inference on academic budgets.
- Decoder-only: learns to minimize $p(x_i | x_{i-1}, x_{i-2}, … x_2, x_1)$ for real sequences of $x$’s. Uses a causal attention mask.
- Given some text, you can sample from p to continue generating realistic text.
4096 token context (8x BERT) by default; has 16K variants.

**Vision Transformers (ViTs)** are an encoder-only transformer architecture for computer vision. They split an image up into 16x16 pixel “patches”, which are then treated as a sequence. They produce dense vector representations for each patch and also a representation for the entire image.

- Many, many pre-trained weights available in many different sizes. Imageomics trained a ViT-B/16 (base, 16x16 pixel patch) for BioCLIP on the Ohio Supercomputer Center. ViT-L/14 (large, 14x14 pixel patch) is likely out of reach for most academic labs. Inference is very cheap.
- Can be used for image classification, object detection, pose estimation, etc.

**Whisper** (from OpenAI) is a family of encoder-decoder transformer models for speech-to-text. The decoder component can be used to sample new tokens conditioned on both previously sampled tokens and the encoder’s representations. Encoder-decoder models are most often used where the output is variable length and is a different modality to the input. This includes speech-to-text, text-to-speech, image-to-text, language translation, and others.

## U

### Unsupervised Learning

As opposed to [supervised learning](#supervised-learning), unsupervised learning detects patterns or structures within the input data without any labels. Clustering and dimensionality reduction techniques are some examples.

## V

### Vision Models

Vision encoder, vision model, image model, and vision backbone are all synonyms used to describe a model that produces dense vector representations for images. Semantically similar images should be close together in this vector embedding space.

### Vision Language Model (VLM)

A model that incorporates both text and images; it may take both as input or output. Examples include [ViT-based](#transformer-examples) [CLIP](#contrastive-language-image-pre-training-clip) models which have both a vision and a text encoder to align images and text in the same embedding space.

## W

## X

## Y

## Z

### Zero-Shot Prediction

Predicting something on which the model was not explicitly trained. For instance, asking [BioCLIP](https://huggingface.co/spaces/imageomics/bioclip-2-demo) to classify a picture of a Pokemon, giving it a list ["pickachu", "ninetails", "evee"]; it was not trained with these labels, nor with images of the Pokemon, but it will still provide an answer. A more practical example, would be new species recognizing species which it did not see in training.
