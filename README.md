# Comp790-166: Computational Biology

## Details
Instructor: Natalie Stanley

Email: natalies@cs.unc.edu

Time: Tuesday/Thursday 9:30am-10:45am, Spring Semester 2021

Office Hours: Thursday 11am-noon on our class zoom link and by appointment. 

Location: **Upate Jan 18: If you have not receieved my welcome email, please send me an email for the zoom link**

## Description
Moden high-throughput assays allow us to efficiently profile a variety biological processes at a systems-level across a set of patient samples. As a result, these technologies generate an abundance of detailed information that needs to be extracted, analyzed and interpreted. In this course we will discuss the methodology used to analyze (process, engineer features from, combine, etc.) data generated by some of the most cutting-edge technologies, such as proteomics, single-cell assays, and imaging in biomedicine.  We will further discuss how numerical linear algebra techniques and modern machine learning approaches can be applied to effectively extract information from these assays for an improved understanding of human health and disease. **While computational biology is a very broad field, we will focus here on the analysis of data generated by single-cell technologies (e.g. mass cytometry), multiomics/multi-modality analysis, systems immunology, and benchmarking.** For each class of algorithms introduced for some task on biological data, we will also go over necessary theory and mathematical intuition. 

## Prerequistes
Strong programming. Comfortable with linear algebra and basic probabilty. Please do not worry if you don't have any background in biology. Any relevant concepts will be introduced. Please feel free to talk to me about any of these prerequistes. 

## Course Structure
This course will be mostly lecture-based with two homework assignments and a course project. I will provide ideas for several publicly available biological datasets and open problems for you to work on for these projects. Overall, the project is intended to give you an opportunity to implement/apply methodology discussed in the papers that we will discuss together. The final project writeup will also give you practice writing up results and communicating ideas. You are welcome to work on teams for this project.

Most of the lectures will be based around several papers. To benefit your own understanding, I will provide a set of questions that should be answered for one of the papers discussed in each lecture.

# Schedule

Note that this is preliminary. Some topics may take (on average) 1 day longer than planned. **I reserve the right to correct typos in the notes up to 1hr before our class meeting.** 

| Date | Topic | Reading | Notes | Code |
|------|-------|---------|-------|------|
| Jan 19, 2021    | Intro, bioinformatics vs comp bio, challenges and modality-specific advancements     | [[Systems Immunology, Just Getting Started](https://pubmed.ncbi.nlm.nih.gov/28632713/)] | [Lecture 1 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture1_handout.pdf) | | |
| Jan 21, 2021   | Linear Algebra Review, Low Rank Approximations, Building graphs from data, Graph Laplacian | [[SLMP. pages 10-22](https://arxiv.org/abs/2004.07984)], [[Data Matrices + Low Rank](https://arxiv.org/abs/1705.07474)], [[Random Projection Trees](https://cseweb.ucsd.edu/~dasgupta/papers/rptree-stoc.pdf)],[[LargeVis](https://arxiv.org/abs/1602.00370)] **no reading summary** | [Lecture 2 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture2_handout.pdf)  | [[LargeVis](https://github.com/lferry007/LargeVis)][[graph tools for python](https://github.com/KrishnaswamyLab/graphtools)] |
| January 26, 2021 | Graph Partitioning |  [[Module Detection Benchmarking in Biological Data](https://www.nature.com/articles/s41592-019-0509-5)], [[BigClam](https://cs.stanford.edu/people/jure/pubs/bigclam-wsdm13.pdf)]. **for fun**: [[Stochastic Block Model + Single Cell](https://www.biorxiv.org/content/10.1101/2020.06.28.176180v1.full)], | [Lecture 3 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture3_handout.pdf)  | [[SNAP](https://snap.stanford.edu/)], [[Louvain](https://github.com/vtraag/louvain-igraph)], [[Leiden](https://github.com/vtraag/leidenalg)], [[graph-tool (SBM)](https://graph-tool.skewed.de/)]. |
| January 28, 2021 | Graph partitioning (overflow slides), Graph Embeddings, Graph Signal Procssing | [[Node2Vec](https://dl.acm.org/doi/pdf/10.1145/2939672.2939754?casa_token=vQTboPUL6qIAAAAA:XQsAUtXd4MyWfj1ClUBw8FKhuPbpqO-aE2d7EDs5iX9-jJZP9BuxDbKUjg3CM69YKHALjCAKJtJx)], [[Representation Learning on Graphs](https://arxiv.org/abs/1709.05584)], [[Review: Graph Embedding in Comp Bio](https://www.frontiersin.org/articles/10.3389/fgene.2019.00381/full)], **for fun**: [[Review on GSP](https://arxiv.org/abs/1211.0053)], [[Low Pass Filtering on Graphs](https://arxiv.org/abs/2008.01305)], [[Vicus](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005621)], [[Mashup](https://www.cell.com/cell-systems/fulltext/S2405-4712(16)30360-X?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS240547121630360X%3Fshowall%3Dtrue)] | [Lecture 4 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture4_hanodut.pdf) | [[node2vec](https://github.com/aditya-grover/node2vec)]|
| February 2, 2021 | Single Cell Day 1: Intro to single-cell profiling, mass cytometry bioinformatics | [[Single-Cells, Many Features](https://www.sciencedirect.com/science/article/pii/S009286741630410X)], [[Spade](https://www.nature.com/articles/nbt.1991)] | [Lecture 5 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture5_handout.pdf) | [[FCS file tutorial](https://github.com/stanleyn/fcs_tutorial)], [[Spade](https://github.com/nolanlab/spade)] |
| February 4, 2021 : **[[HW 1 Assigned](https://github.com/stanleyn/Comp790-166-Comp-Bio/tree/main/Homework1)]** | Single Cell Day 2: Graph-based automated gating, imputation in single-cell data, branch-point preserving visualization | [[phenograph](https://www.sciencedirect.com/science/article/pii/S0092867415006376)], [[PHATE](https://www.nature.com/articles/s41587-019-0336-3)], [[MAGIC](https://www.biorxiv.org/content/10.1101/111591v1)] | [Lecture 6 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture6_handout.pdf) | [[phenograph](https://github.com/JinmiaoChenLab/Rphenograph)],  [[FastPG](https://github.com/sararselitsky/FastPG)], [[MAGIC](https://github.com/KrishnaswamyLab/MAGIC)], [[Phate](https://github.com/KrishnaswamyLab/PHATE)] |
|February 9, 2021 | Single Cell Day 3: Geometry Based Data Generation, Denoising, Data Augmentation + Linking Single-Cell Data to External Variables | [[SUGAR](https://arxiv.org/abs/1802.04927)], [[MELD](https://www.biorxiv.org/content/10.1101/532846v4)] | [Lecture 7 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture7_public.pdf) | [[Meld](https://github.com/KrishnaswamyLab/MELD)], [[sugar](https://github.com/stanleyjs/sugar)] |
| February 11, 2021 | Single Cell Day 4: Graph Fourier Transform , Low Pass Filtering, Finish up MELD, Differential Abundance Analysis of Cell Populations |  **for fun**: [[Low Pass Filtering on Graphs](https://arxiv.org/abs/2008.01305)] | [Lecture 8 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture8_public.pdf) | [[GSP toolbox](https://pygsp.readthedocs.io/en/stable/)] | 
| February 16, 2021 | **Wellness day no class** | 
| February 18, 2021 : **Homework 1 Due** | Single Cell Day 5: Differential Analysis of Cell Populations + Projecting Data According to Background Variance | [[Contrastive PCA](https://www.nature.com/articles/s41467-018-04608-8)], [[Cydar](https://www.nature.com/articles/nmeth.4295)], [[Milo](https://www.biorxiv.org/content/10.1101/2020.11.23.393769v1)] | [Lecture 8 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture9_public.pdf) | [[cPCA](https://github.com/abidlabs/contrastive), [[Milo](https://github.com/MarioniLab/miloR)], [[cydar](https://www.bioconductor.org/packages/release/bioc/html/cydar.html)] |
| February 23, 2021  | Single Cell Day 7:  **Guest lecture by [Maria Brbic (Stanford CS)](https://cs.stanford.edu/~mbrbic/)** : Semi-Supervised Automated Cell-Population Discovery  | MARS| 
| February 25, 2021 | Single Cell Day 6: Combinging Multiple Single-Cell Datasets | [[Conos](https://www.nature.com/articles/s41592-019-0466-z)], SAUCIE|
| March 2, 2021 | Single Cell Day 7: Trajectory Inference | |
| March 4, 2021 | Single Cell Day 8: Benchmarking in Trajectory Inference | |
| March 9, 2021 : **Project Proposals Due** | Presentations of Project Propsals Day 1 | |
| March 11, 2021  | **Wellness Day no class**  | |
| March 16, 2021 | Project Proposal Presentation Day 2 | |
| March 18, 2021  | Single Cell Day 9: Benchmarking in Single-Cell Analysis | Aghaeepour et al |
| March 23, 2021 | Single Cell Day 10: Imaging Proteomics + Spatial Regularization : computational challeneges in combining tissue images and protein expression | |
| March 25, 2021 | Multiomics Day 1: Constructing a joint embedding of samples according to multiple modalities, subspace merging | SNF, grassmann embed |  
| March 30, 2021 | Multiomics Day 2: MOFA-1 and MOFA-2: Multiomics Factor Analysis | MOFA-1, MOFA-2 | 
| April 2, 2021 : **HW 2 Assigned** | Multiomics Day 3: Uncovering Relationships Between Modalities | mmvec| 
| April 6, 2021 | Multiomics Day 4: Stacked Generalization and CCA in multiomics studies | Ghaemi |
| April 8, 2021 | Multiomics Day 5: Benchmarking in multiomics studies | |
|April 13, 2021  | Incorporating Prior Biological Knowledge into Analysis | |
|April 15, 2021 : **Homework 2 Due** |  Systems Immunology Topic: TCR/BCR (T and B cell receptor reperotire analysis) | | 
|April 20, 2021 | Partial Correlation, Thresholding etc for Identifying Meaningful Interactions | | 
|April 22, 2021 | Enrichment Analysis, writing for an interdiscplinary audience | | 
|April 27, 2021 | Project Presentations Day 1 | |
|April 29, 2021 | Project Presentations Day 2 | |
|Final Exam Day | Project papers due | |

# Homework, Project, Reading, Grading, Etc

## Homework
There will be two homework assignments to practice implementing particular concepts. Often, things can become a bit easier to understand and use when they are implemented by you. I will be happy to read/run code written in Python, R, Julia, or Matlab. Please submit your homework writeup as a PDF. 

## Background Resources
Most of what we discuss in class will come from papers. However, I suggest the following textbooks as background references. Conveniently, they are also available for free.

* [PRML] Pattern Recognition and Machine Learning-- Chris Bishop [[Link](http://users.isr.ist.utl.pt/~wurmd/Livros/school/Bishop%20-%20Pattern%20Recognition%20And%20Machine%20Learning%20-%20Springer%20%202006.pdf)]

* [SLMP] Spectral Learning on Matrices and Tensors -- Majid Janzamin et al. [[Link](https://arxiv.org/abs/2004.07984)]

* The Matrix Cookbook [[Link](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf)]

* [PML] Probabilistic Machine Learning: An Introduction. -- Kevin Murphy [[Link](https://probml.github.io/pml-book/book1.html)]

## Readings
For each class, I will update the papers that we will go over in above table. You will only be required to write a summary of one of the potentially multiple papers assigned for that day.

### Reading Questions

**Please choose one paper per week on the weeks when reading summaries are due and turn them in before our class meeting 9:30 am to natalies+comp790@cs.unc.edu**. 

1) Please explain in 2 sentences or less what the problem being solved is.

2) What were the main contributions of the authors in this work? (You can answer in a few bullet points). 

3) Please describe 1-2 computational experiments that the authors implemented to test their method.

4) Were the authors the first to attempt this particular problem? If not, did they compare their results to other baselines? Do you think that their evaluation was objective?

5) Do you think that the authors provided enough evidence for why their developed method is an important contribution? If yes, please describe their reasoning here. If you do not think they adequately justified why they worked on this particular problem, please describe your thoughts on that here. 

6) What is one follow-up idea or extension from this work? 

## Final Project
I will provide you with several examples of publicly available biological datasets and problems (https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Datasets.md). Half-way through the semester, you will submit your project proposal and present your idea to the class.  The proposal will be a short document describing 1) The problem 2) A background on other people's attempts to solve this problem and 3) A background on your idea of a solution and 4) the data you will use to test your method. At the end of the semester you will write a short paper explaining your method and results and present your results.

## Grading
 Grading will be based on the following

1) Reading Questions : 20% over the entire semester
2) Homework 1: 20%
3) Homework 2: 20%
4) Project Proposal : 10%
5) Project final writeup: 30%

## Accessibility Statement
The University of North Carolina at Chapel Hill facilitates the implementation of reasonable accommodations, including resources and services, for students with disabilities, chronic medical conditions, a temporary disability or pregnancy complications resulting in barriers to fully accessing University courses, programs and activities.
Accommodations are determined through the Office of Accessibility Resources and Service (ARS) for individuals with documented qualifying disabilities in accordance with applicable state and federal laws. See the ARS Website for contact information: https://ars.unc.edu or email ars@unc.edu.

(source: https://ars.unc.edu/faculty-staff/syllabus-statement)

## Diversity Statement
I value the perspectives of individuals from all backgrounds reflecting the diversity of our students. I broadly define diversity to include race, gender identity, national origin, ethnicity, religion, social class, age, sexual orientation, political background, and physical and learning ability. I strive to make this classroom an inclusive space for all students. Please let me know if there is anything I can do to improve, I appreciate suggestions.
