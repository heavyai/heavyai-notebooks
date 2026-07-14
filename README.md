# heavyai-notebooks
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/heavyai/heavyai-notebooks/blob/main/LICENSE)
[![Security](https://img.shields.io/badge/Security-Report%20a%20Vulnerability-red.svg)](https://github.com/heavyai/heavyai-notebooks/blob/main/SECURITY.md)
[![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-blue?logo=github)](https://github.com/orgs/heavyai/discussions)



Example Python notebooks for use with the HeavyAI analytics platform

The file `environment.yml` describes a minimal conda/mamba environment that can
be used to execute the notebooks.

The following assumes that you have an instance of HeavyAI running.
UDFs and UDTFs are enabled with the flags
`--enable-runtime-udfs` and `--enable-table-functions`. For more information on
installing HeavyAI, see
[here](https://docs.HeavyAI/installation-and-configuration/installation). 

To summarize:

```bash
# works with mamba too
conda env create -f environment.yml
conda activate heavyai-env

# if you need to run heavydb locally
conda install heavydb  # only linux and windows, use docker on macOS
mkdir -p data
initheavy data -f
heavydb --enable-runtime-udfs --enable-table-functions
```


## Security
> [!WARNING]
> **Do not report security vulnerabilities through public GitHub issues!**

NVIDIA takes security seriously. If you discover a vulnerability in heavyai-notebooks, **DO NOT open a public issue**. Use one of the private reporting channels described in [SECURITY.md](https://github.com/heavyai/heavyai-notebooks/blob/main/SECURITY.md).

## Support
Join the [HeavyAI GitHub Discussions](https://github.com/orgs/heavyai/discussions) to ask questions, share feedback, and report issues. HeavyAI maintainers review issues, discussions, and pull requests on a best effort basis without guaranteed response timelines.
  
## License
Apache 2.0. See [LICENSE](https://github.com/heavyai/heavyai-notebooks/blob/main/LICENSE).
