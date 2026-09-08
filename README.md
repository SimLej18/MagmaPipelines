# ⚠️ Important notice ⚠️

If you are looking to run the MagmaClust algorithm with a Python implementation, **[the Mimosa package](https://github.com/UNamurCSFaculty/mimosa-ml) is the way!** It is fully-featured, more stable, less buggy and actively maintained by Magma's original team!

# Examples of usage of the MagmaClustPy package

This repo contains notebooks presenting the minimal steps involved in training
a Magma or MagmaClust model, using the [MagmaClustPy package](https://github.com/SimLej18/MagmaClustPy).

Note that the package is in heavy development. Most features are not fully stable.

## Installation

You can run the library using conda with the wollowing commands:

```bash
conda create -n magma python=3.12
conda activate magma
pip install -r requirements.txt
```

Then you'll be able to execute and play with the various notebooks in the repository.

## Status of the pipelines:

* ✅ **Magma** - Distinct inputs among tasks, Shared hyper-parameters
* ✅ **Magma** - Distinct inputs among tasks, Distinct hyper-parameters
* ⚠️ **Magma** - Shared inputs among tasks, Shared hyper-parameters
  * mean-process hyper-parameters do not converge to the expected mean-process
* ⚠️ **Magma** - Shared inputs among tasks, Distinct hyper-parameters
  * mean-process hyper-parameters do not converge to the expected mean-process
* ❌ **MagmaClust** - Distinct hyper-parameters, No cluster hyper-parameters
  * bug when predicting new tasks
* ❌ **MagmaClust** - Distinct hyper-parameters, Cluster hyper-parameters
  * bug when predicting new tasks
* ✅ **MagmaClust** - Shared hyper-parameters, No cluster hyper-parameters
  * ⚠️ weird behavior when predicting away from data
* ✅ **MagmaClust** - Shared hyper-parameters, Cluster hyper-parameters
  * ⚠️ weird behavior when predicting away from data

---
