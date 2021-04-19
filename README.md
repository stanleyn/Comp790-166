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
| February 18, 2021| **Class Canceled due to Weather** |
| February 23, 2021 : **Homework 1 Due**, [[**Project Proposal Template**](https://github.com/stanleyn/Comp790-166-Comp-Bio/tree/main/Projects)] | Single Cell Day 5:  **Guest lecture by [Maria Brbic (Stanford CS)](https://cs.stanford.edu/~mbrbic/)** : Semi-Supervised Automated Cell-Population Discovery  | [[MARS](https://www.nature.com/articles/s41592-020-00979-3)]| No slides | [[MARS](https://github.com/snap-stanford/mars)] | 
| February 25, 2021  | Single Cell Day 6: Differential Analysis of Cell Populations + Projecting Data According to Background Variance | [[Contrastive PCA](https://www.nature.com/articles/s41467-018-04608-8)], [[Cydar](https://www.nature.com/articles/nmeth.4295)], [[Milo](https://www.biorxiv.org/content/10.1101/2020.11.23.393769v1)] | [Lecture 9 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture9_public.pdf) | [[cPCA](https://github.com/abidlabs/contrastive)], [[Milo](https://github.com/MarioniLab/miloR)], [[cydar](https://www.bioconductor.org/packages/release/bioc/html/cydar.html)] |
| March 2, 2021 : **Reading Summary 2 Due by Today**| Single Cell Day 7: Combinging Multiple Single-Cell Datasets | [[Conos](https://www.nature.com/articles/s41592-019-0466-z)], [[CytofMerge](https://academic.oup.com/bioinformatics/article/35/20/4063/5381543)], [[Harmony](https://www.biorxiv.org/content/10.1101/461954v2.full.pdf)], [[SAUCIE](https://www.nature.com/articles/s41592-019-0576-7)],| [Lecture 10 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture10_handout.pdf) | [[Conos](https://github.com/kharchenkolab/conos)], [[CyTOFMerge](https://github.com/tabdelaal/CyTOFmerge)] | 
| March 4, 2021 | Single Cell Day 8: Combining Multiple Panels, Starting Pseudotime and Mapping Cellular Differentiation | [[Diffusion Maps for Differentiation](https://academic.oup.com/bioinformatics/article/31/18/2989/241305)], [[SLICER-developed at UNC](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0975-3)], [[Original Diffusion Maps (Coifman)](https://papers.nips.cc/paper/2005/file/2a0f97f81755e2878b264adf39cba68e-Paper.pdf)] | [Lecture 11 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture11_public.pdf) | [[Diffusion Maps -Scanpy](https://scanpy.readthedocs.io/en/latest/api/scanpy.tl.diffmap.html)], [[SLICER](https://github.com/jw156605/SLICER)] | 
| March 9, 2021 : **Project Proposals Due**, [Sign up for a presentation slot!](https://docs.google.com/spreadsheets/d/1puFjmjadZuuVIy6nyJJPHJbucrW4-KH-xFd2P3HjIEI/edit?usp=sharing) | Combining Multiple Modalities for a common set of patients | [[Subspace Merging on Grassmann Manifold](https://academic.oup.com/bioinformatics/article/35/10/1653/5134062?login=true)], [[Rayleigh Ritz Business (Spectral Clustering...](https://arxiv.org/abs/0711.0189)] | [Lecture 12 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture11_public.pdf) | [[Grassmann Cluster](https://github.com/michaelsharpnack/GrassmannCluster)] |
| March 11, 2021  |**Wellness Day no class**  | |
| March 16, 2021  | Presentations of Project Propsals Day 1  | |
| March 18, 2021 | Project Proposal Presentation Day 2 | |
| March 23, 2021  | Finish Grassmann Embedding, Longitudinal Multimodal Data Integration | [[Longitudinal Multiomodal Data Integration on ADNI](http://psb.stanford.edu/psb-online/proceedings/psb20/Brand.pdf)] | [Lecture 13 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture13_public.pdf) | 
| March 25, 2021 | Finish Longitudinal Multiomodal Data Integration, Brief Journey in Convex Optimization, ADMM | [[ADMM by Stephen Boyd](https://web.stanford.edu/~boyd/papers/pdf/admm_distr_stats.pdf)] | [Lecture 14 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture14_public.pdf) | [[CVX](https://www.cvxpy.org/examples/)] |
| March 30, 2021 | MOFA methods for multiomics integration (both multiple modalities and multiple single-cell!) | [[MOFA](https://www.embopress.org/doi/full/10.15252/msb.20178124)], [[MOFA+](https://link.springer.com/content/pdf/10.1186/s13059-020-02015-1.pdf)] | [Lecture 15 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture15_public.pdf) | [[MOFA](https://github.com/bioFAM/MOFA)] | 
|April 1, 2021 | Integrating multiple heterogeneous graphs (e.g. multiple relational definitions). Start network alignment. | [[Mashup](https://www.cell.com/cell-systems/fulltext/S2405-4712(16)30360-X?)], [[REGAL (network alignment)](https://gemslab.github.io/papers/heimann-2018-regal.pdf)] | [Lecture 16 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture16_public.pdf) | [[REGAL](https://github.com/GemsLab/REGAL)] | 
| April 6 2021 | Refining Graph Alignments, Graph Summarization | [[Refining Network Alignment](https://gemslab.github.io/papers/heimann-2021-RefiNA.pdf)], [[Bridging Network Alignment and Summarization](https://gemslab.github.io/papers/jin-2019-latent.pdf)]  | [Lecture 17 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture17_public.pdf) | [[RefiNA](https://github.com/GemsLab/RefiNA)] | 
|April 8, 2021 : **[[HW 2 Assigned](https://github.com/stanleyn/Comp790-166-Comp-Bio/tree/main/Homework2)]** | Harmonic alignment for multimodal single cell data, graph neural networks vs label propagation + correction  | [[Harmonic Alignment + Single Cell Multimodal](https://epubs.siam.org/doi/pdf/10.1137/1.9781611976236.36)], [[Learning on Graphs- Correct and Smooth](https://openreview.net/pdf?id=8E1-f3VhX1o)] | [Lecture 18 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture18_public.pdf) |
| April 13, 2021 :  | Computational Neuroscience + Time Varying Analysis of Brain Connectivity | [[review on chronnectome](https://www.sciencedirect.com/science/article/pii/S0896627314009131)], [[edge functional connectivity](https://www.nature.com/articles/s41593-020-00719-y.pdf)], [[Edge Communities + Brain Connectivity](https://www.biorxiv.org/content/10.1101/2020.05.05.067777v1.full.pdf)], [[Edge-Level Features](https://www.biorxiv.org/content/10.1101/2021.01.07.425450v1.full.pdf)], [[Predictive Subnetwork Extraction](https://link.springer.com/content/pdf/10.1007%2F978-3-319-46720-7_21.pdf)] | [Lecture 19 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture19_public.pdf) |
| April 15, 2021 | Imaging Proteomics and Genomics + Spatial Regularization | [[LEAPH](https://www.biorxiv.org/content/10.1101/2020.10.02.322529v3.full.pdf)], [[MIBI + TB granuloma](https://www.biorxiv.org/content/10.1101/2020.06.08.140426v1.full.pdf)], [[SpiceMix](https://www.biorxiv.org/content/biorxiv/early/2020/11/30/2020.11.29.383067.full.pdf)] [[Histocat](https://www.nature.com/articles/nmeth.4391)],  | [Lecture 20 Notes](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Lecture_Notes/Lecture20_public.pdf) | 
| April 20, 2021 [[Project Presentation Sign-up](https://docs.google.com/spreadsheets/d/1bSZByipJJxlRGXNqECi02VHxbS39WV6-cXL0akbA2kI/edit?usp=sharing)], [[Project write-up template, TeX available in Projects Folder too](https://github.com/stanleyn/Comp790-166-Comp-Bio/blob/main/Projects/Project_writeup.pdf)]  | Sketching Single-Cell and Biological Datasets  | |
|April 22, 2021 : **Homework 2 Due on April 23**  | Technical Writing in Comp Bio. Summary of What we Covered | |
|April 27, 2021 :  |  Project Presentations Day 1 | | 
|April 29, 2021 | Project Presentations Day 2 | |
|May 4, 2021 | Project Presentations Day 3 | |
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
