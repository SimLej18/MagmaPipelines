# Examples of usage of the MagmaClustPy package

This repo contains notebooks presenting the minimal steps involved in training
a Magma or MagmaClust model, using the [MagmaClustPy package](https://github.com/SimLej18/MagmaClustPy).

Note that the package is in heavy development. Most features are not fully stable.

## Status of the pipelines:

* ✅ **Magma** - Distinct inputs among tasks, Shared hyper-parameters
* ✅ **Magma** - Distinct inputs among tasks, Distinct hyper-parameters
* ⚠️ **Magma** - Shared inputs among tasks, Shared hyper-parameters
  * mean-process hyper-parameters do not converge to the expected mean-process
* ⚠️ **Magma** - Shared inputs among tasks, Distinct hyper-parameters
  * mean-process hyper-parameters do not converge to the expected mean-process
* ❌ **MagmaClust** - Distinct hyper-parameters, No cluster hyper-parameters
  * bug chen predicting new tasks
* ❌ **MagmaClust** - Distinct hyper-parameters, Cluster hyper-parameters
  * bug chen predicting new tasks
* ✅ **MagmaClust** - Shared hyper-parameters, No cluster hyper-parameters
  * ⚠️ weird behavior when predicting away from data
* ✅ **MagmaClust** - Shared hyper-parameters, Cluster hyper-parameters
  * ⚠️ weird behavior when predicting away from data

---