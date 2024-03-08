# AdvOcl: Naturalistic Clothing Pattern Adversarial to Person Detectors in Occlusion


* AdvOcl leverages the learned image manifold of
the diffusion model to generate patterns that resemble one kind of
the typical textures of daily clothes, such as common floral styles and improves the adaptability capacity and adversarial effectiveness by supporting changes in posture and partially
occlusion during walking or running with warping and alignment
module modeling deformation of clothes.
## Set the env
```python
conda create -n AdvOcl python=3.8

git clone https://github.com/lluzt/AdvOcl

cd AdvOcl

pip install -r requirements.txt
```

## Datasets
We train the models on small sets of dimension 5.
Train/val/test sets use disjoint classes by default.


* `CIFAR100` - (3 x 32 x 32) - 60/20/20


We convert the original data [VITON](https://github.com/xthan/VITON) into different directories for easily use.



## Training

Train a FSDM on CIFAR100

```bash
sh script/run.sh gpu_num
```



## Acknoledgments

A lot of code and ideas borrowed from:

* https://github.com/georgosgeorgos/few-shot-diffusion-models
* https://github.com/xthan/VITON
* https://gitlab.com/EAVISE/adversarial-yolo


