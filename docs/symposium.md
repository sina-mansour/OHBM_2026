# Balancing Sample Size and Sensitivity: Emerging Methods and Tools for Optimal Inference & Power Analysis

🎙️ **OHBM 2026 Symposium**  
📍 **Location**: Palais 2 l’Atlantique, Bordeaux, France  
🗓️ **Date**: Wednesday, 17 Jun 2026
⏰ **Time**: 11:30 - 12:45

---

## Organisers

- **Martin Lindquist**, Johns Hopkins University, USA
- **Sina Mansour L.**, National University of Singapore & The University of Melbourne
- **Stephanie Noble**, Northeastern University, USA
- **Camille Maumet**, Inria, France

## Speakers

- **Niousha Dehestani**, National University of Singapore
- **Hallee Shearer**, Northeastern University, USA
- **Selena Wang**, Indiana University, USA
- **Nick Yao Larsen**, Aarhus University, Denmark

---

## Overview

Robust statistical inference is foundational to meaningful interpretation of fMRI findings, yet many existing pipelines remain ill-equipped to detect distributed, network-level effects, accurately estimate effect sizes, or to characterise dynamic brain processes under realistic sample-size constraints. This symposium brings together emerging methods, analytical frameworks, and openly accessible software that directly address these limitations — spanning spectral inference, effect size benchmarking, latent-space network analysis, and statistical testing of brain dynamics. Collectively, the presentations demonstrate how leveraging large-*n* open datasets, principled priors, and modern statistical tools can substantially improve sensitivity, reliability, and interpretability without requiring prohibitively large cohorts.

The symposium follows a four-talk format with a moderated panel discussion at the end, encouraging synthesis across complementary methodological perspectives.

---

## Talks

### SPARC: A Spectral Framework for Power-Enhanced, Multiple-Comparison-Corrected fMRI Inference

**Niousha Dehestani** *(National University of Singapore)*

Reliable detection of task-evoked activation in fMRI remains challenging due to low effect sizes, spatially structured noise, and limited cohort sizes. Conventional multiple-testing correction methods typically improve sensitivity by clustering local high-magnitude signals, but they fail to capture distributed activation patterns that span non-contiguous cortical and subcortical regions, a hallmark of large-scale network organisation in the brain.

To address this limitation, we propose a spectral permutation inference framework (**SPARC**) that leverages brain connectivity eigenmodes to enhance the statistical power of inference at the level of voxels/vertices. SPARC projects group-level statistical maps into a low-dimensional spectral basis, filtering out high-frequency components that are more likely to be contaminated by noise while retaining structured neural signals. We evaluate three spectral representations: (1) structural eigenmodes derived from white-matter connectivity, (2) functional eigenmodes derived from resting-state functional coactivation structure, and (3) hybrid eigenmodes integrating both sources of brain connectivity organisation.

Benchmarked across multiple Human Connectome Project task paradigms and varying sample sizes, spectral inference via the hybrid eigenmode basis consistently outperforms traditional permutation-based corrections, yielding **20–35% improvements in statistical power** and a ~20% increase in Bookmaker Informedness, confirming that sensitivity gains do not inflate false positives. These results demonstrate that spectral inference, particularly when incorporating hybrid structure–function organisational principles, increases statistical power for the detection of distributed brain activation patterns, ultimately supporting stronger fMRI inference with smaller sample sizes.

---

### Modeling the cross-brain distribution of effect sizes

**Hallee Shearer** *(Northeastern University, USA)*

Emerging reports suggest that sample sizes commonly used in functional neuroimaging studies may be too small to detect many brain–behaviour relationships, posing a major barrier to brain and mental health research. A central challenge is that planning robust studies requires researchers to know what effect sizes to expect, yet this essential information is surprisingly difficult to estimate in practice and thus often omitted from study planning. In particular, standard "mass univariate" procedures for estimating effects across multiple brain areas simultaneously give an inflated picture of how large effect sizes are.

Here, we introduce a method to correct this inflation bias and perform an unprecedented analysis of **63 studies across seven large datasets** (n = 100–40,000; 52,979 total participants) to establish effect size benchmarks in functional neuroimaging. We also provide an interactive web application to facilitate the exploration of these effect size benchmarks.

We find that between-subjects effects are exceedingly small at the majority of brain areas, requiring sample sizes beyond typical consortia (*n* > 100–5,000 for 80% statistical power) to detect even the very strongest voxel- or edge-level effects. However, multivariate analyses and within-subject task designs can yield substantially larger effect sizes that can be detected at sample sizes within reach of most labs (*n* < 25–50). By establishing data-driven effect size benchmarks, these findings lay the groundwork for more informed study planning in neuroscience while highlighting shared challenges — and the potential for shared solutions — across biomedicine.

---

### Improve power efficiency of brain-behavior studies using LatentSNA

**Selena Wang** *(Indiana University, USA)*

The brain is comprised of interacting neurons, and its complexity poses significant challenges for researchers to understand its structure, function, and dynamics. Latent-space-based network analysis, a collaboration between network science and statistics, has emerged as a powerful tool for understanding the generative process of such interconnected systems and for performing statistical inference and prediction.

With **LatentSNA** (latent variables-assisted statistical network analysis), we substantially improve the statistical power for identifying biomarkers, and as a result, we discover large, star-like brain functional architectures implicated in the development of internalising symptoms in **5,000 to 7,000 children** of the Adolescent Brain Cognitive Development (ABCD) study. This finding supports internalising as a complex and evolving psychological phenomenon whose development involves large-scale affective interference of multiple coordinating functional systems. The proposed methods have broad applicability and can contribute to many domains of science with rigorous and powerful analysis.

---

### A comprehensive framework for statistical testing of brain dynamics

**Nick Yao Larsen** *(Aarhus University, Denmark)*

We introduce a comprehensive statistical framework for analysing brain dynamics and testing their associations with behavioural, physiological, and other non-imaging variables. Based on a generalisation of the Hidden Markov Model (HMM) — the **Gaussian-Linear HMM** — our open-source Python package supports multiple experimental paradigms, including task-based and resting-state studies, and addresses a wide range of questions in neuroscience and related scientific fields.

The toolbox is available as both a Python library and a graphical interface, so it can be used by researchers with or without programming experience. Statistical inference is performed using permutation-based methods and structured Monte Carlo resampling, and the framework can easily handle confounding variables, multiple testing corrections, and hierarchical relationships within the data, among other features. The package includes tools for intuitive visualisation of statistical results, along with comprehensive documentation and step-by-step tutorials. Altogether, it provides a broadly applicable, end-to-end pipeline for analysis of functional neural data and its dynamics.

---

## Format

Four 15-minute presentations followed by a 15-minute moderated panel discussion with audience participation, balancing focused methodological talks with integrative cross-method synthesis.