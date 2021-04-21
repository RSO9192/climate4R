## conda recipe for the climate4R core packages

To install the whole framework go to [conda-full](https://github.com/SantanderMetGroup/climate4R/tree/devel/conda-full)

```bash
# create a conda environment
conda create --name nameofmycondaenvironment
# activate the environment
conda activate nameofmycondaenvironment
# install climate4R
conda install -c defaults -c r -c conda-forge -c santandermetgroup climate4r-base=1.0.1
```
Activate the conda environment to work with climate4R. To deactivate the environment run the following:

```bash
# deactivate the environment
conda deactivate
```

### Build (only for the admin)

```bash
conda build -c defaults -c r -c conda-forge .
anaconda login
anaconda upload -u SantanderMetGroup TAR_BZ2
```
