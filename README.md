# Projects
A collection of some of the projects I have finished with others during my time as a masterstudent Artificial Intelligence at the University of Amsterdam

## Registers in Small Vision Transformers: A Reproducibility Study of Vision Transformers Need Registers (Publication)
### Abstract
Recent work has shown that Vision Transformers (ViTs) can produce “high-norm” artifact
tokens in attention maps. These artifacts disproportionately accumulate global information,
can degrade performance, and reduce interpretability in these models. Darcet et al. (2024)
proposed registers—auxiliary learnable tokens—to mitigate these artifacts. In this repro-
ducibility study, we verify whether these improvements extend to smaller ViTs. Specifically,
we examine whether high-norm tokens appear in a DeiT-III Small model, whether registers
reduce these artifacts, and how registers influence local and global feature representation.
Our results confirm that smaller ViTs also exhibit high-norm tokens and registers partially
alleviate them, improving interpretability. Although the overall performance gains are mod-
est, these findings reinforce the utility of registers in enhancing ViTs while highlighting open
questions about their varying effectiveness across different inputs and tasks. Our code is
available at https://github.com/SnorrenanxD/regs-small-vits.
### [Link](https://openreview.net/forum?id=5JflRlCt3Q)

## 3D Hand Contact Estimation from 2D Foundation Models
### Abstract
Estimating dense 3D contact between hands and objects
from a single monocular RGB image is a core challenge
in dexterous interaction understanding. We present a
method for predicting binary contact maps over MANO
hand meshes directly from RGB input, without access to
depth or object geometry at test time. Our approach fine-
tunes InteractVLM: a model that grounds vision-language
semantic representations into 3D meshes, on the ARCTIC
bimanual manipulation dataset, adapting it from full-body
contact estimation to the hand domain. The pipeline ren-
ders MANO hand meshes into multi-view canonical images,
produces 2D contact masks using a shared encoder con-
ditioned on VLM features, and lifts these contact masks
to binary per-vertex 3D contact labels via a precomputed
pixel-to-vertex lookup table. The LISA-13B backbone [12]
is fine-tuned with low-rank adaptation while the SAM mask
decoder [10] is jointly trained to adapt from general seg-
mentation to MANO contact prediction. Experiments on
ARCTIC demonstrate the viability of adapting a full-body
VLM contact estimation framework to the hand domain.
### [Link](3D_Hand_Contact_Estimation.pdf)

## Evaluating the Brain Predictivity of Text Embeddings: A Comparison Between Large Language Models and Text Embedders
### Abstract
Brain encoding studies of language have largely
relied on autoregressive, decoder-only large
language models (LLMs), extracting passage-
level representations via heuristics such as
last-token or mean pooling. Dedicated text
embedders, fine-tuned from LLM backbones
with contrastive or instruction-following ob-
jectives, are designed to produce semantically
dense passage-level representations, yet re-
main largely unevaluated as models of neu-
ral language processing. We compare Qwen3-
Embedding against the matched decoder-only
Qwen3 at three sizes (0.6B, 4B, 8B), predicting
fMRI responses from the Pereira et al. (2018)
dataset in the left-hemisphere language net-
work. Across both experiments and all sizes,
the two model families exhibit distinct layer-
wise brain-predictivity profiles: the embedder
peaks in early-to-mid layers while the LLM
peaks in late layers, despite sharing the same
causal attention architecture. A Toneva resid-
ual analysis further shows that the two archi-
tectures carry partially complementary brain-
relevant information. These results suggest that
training objective, rather than attention direc-
tionality, shapes how text-level semantic infor-
mation is distributed across layers, and that
dedicated embedders are competitive candidate
models of passage-level neural language repre-
sentations.
### [Link](Evaluating_Brain_Predictivity.pdf)

## Language Identification using Transformer-based Architectures: A Comparative Study with mBERT and downstream classifiers
### Abstract
Language Identification (LID) is a foundational
task in Natural Language Processing (NLP)
that determines the language of a given text.
In this study, we evaluate three Transformer-
based approaches to LID using the WiLI-2018
benchmark dataset. We employ mBERT as a
shared encoder and compare the effectiveness
of (i) a linear classification head as baseline,
(ii) an MLP classifier, and (iii) a CNN classifier.
Our results suggest that more complex down-
stream architecture choices do not yield notable
performance improvements in LID tasks. We
evaluate all three models on standard metrics,
provide an in-depth error analysis, and express
actionable future work directions.
### [Link](LID_using_Transformer_based_Architectures.pdf)

## Leveraging Scale Equivariant Graph MetaNetworks to Classify and Repair Poisoned Networks
### Abstract
The Scale Equivariant Graph MetaNetwork (ScaleGMN) was introduced by
Kalogeropoulos et al. [2024] based on scaling symmetries in feedforward neural
networks. to generalize feedforward neural networks, classify implicit neural repre-
sentations (INRs), and edit these INRs. In this work, we build on this metanetwork
and apply it to trojan detection and cleansing. For this end, we generate trojaned
CNN models trained on poisoned CIFAR10 datasets and use these to train and
test the model for classification and cleansing. resulting in more robust and versa-
tile neural networks. The experiments we have ran can be found an executed in
https://github.com/WouterBesse/scalegmnUvADL2/tree/main
### [Link](SEG_MetaNetworks.pdf)
