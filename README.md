# Projects
A collection of some of the projects I have finished with others during my time as a masterstudent Artificial Intelligence at the University of Amsterdam

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
### [Link] (3D_Hand_Contact_Estimation.pdf)
