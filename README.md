# heavyai-notebooks
Example Python notebooks for use with the HEAVY.AI analytics platform

The file `environment.yml` describes a minimal conda/mamba environment that can
be used to execute the notebooks.

The following assumes that you have an instance of HEAVY.AI running.
UDFs and UDTFs are enabled with the flags
`--enable-runtime-udfs` and `--enable-table-functions`. For more information on
installing HEAVY.AI, see
[here](https://docs.heavy.ai/installation-and-configuration/installation). 

To summarize:

```bash
# works with mamba too
conda env create -f environment.yml
conda activate heavyai-env

# if you need to run heavydb locally
mkdir -p data
initheavy data -f
heavydb --enable-runtime-udfs --enable-table-functions
```
