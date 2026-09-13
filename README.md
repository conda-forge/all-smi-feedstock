About all-smi-feedstock
=======================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/all-smi-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/lablup/all-smi

Package license: Apache-2.0

Summary: Command-line utility for monitoring GPU hardware

Development: https://github.com/lablup/all-smi

all-smi is a command-line utility for monitoring GPU and NPU hardware
across multiple systems. It provides a real-time view of accelerator
utilization, memory usage, temperature, power consumption, and other
metrics, and is designed to be a cross-platform alternative to
nvidia-smi with support for NVIDIA GPUs, AMD GPUs, NVIDIA Jetson
platforms, Apple Silicon GPUs, Intel GPUs, Intel Gaudi NPUs, Google
Cloud TPUs, Tenstorrent NPUs, Rebellions NPUs and Furiosa NPUs.

The application presents a terminal-based user interface with cluster
overview and interactive sorting, for both local and remote monitoring,
and can also export Prometheus metrics via its API mode.

Current build status
====================


<table><tr>
    <td>GitHub Actions</td>
    <td>
      <a href="https://github.com/conda-forge/all-smi-feedstock/actions/workflows/conda-build.yml">
        <img src="https://github.com/conda-forge/all-smi-feedstock/actions/workflows/conda-build.yml/badge.svg?event=push&branch=main">
      </a>
    </td>
  </tr>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=29511&branchName=main">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/all-smi-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=29511&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/all-smi-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-all--smi-green.svg)](https://anaconda.org/conda-forge/all-smi) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/all-smi.svg)](https://anaconda.org/conda-forge/all-smi) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/all-smi.svg)](https://anaconda.org/conda-forge/all-smi) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/all-smi.svg)](https://anaconda.org/conda-forge/all-smi) |

Installing all-smi
==================

Installing `all-smi` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

How to use
----------

<details>
<summary>With conda</summary>

```
conda install all-smi
```

</details>

<details>
<summary>With mamba</summary>

```
mamba install all-smi
```

</details>

<details>
<summary>With pixi</summary>

```
# for adding to your local project
pixi add all-smi
# for installing globally
pixi global install all-smi
```

</details>

Search package versions
-----------------------

It is possible to list all of the versions of `all-smi` available on your platform:

<details>
<summary>With conda</summary>

```
conda search all-smi --channel conda-forge
```

</details>

<details>
<summary>With mamba</summary>

```
mamba search all-smi --channel conda-forge
```

</details>

<details>
<summary>With pixi</summary>

```
pixi search all-smi --channel conda-forge
```

</details>

<details>
<summary>With mamba repoquery, which may provide more information</summary>

```
# Search all versions available on your platform:
mamba repoquery search all-smi --channel conda-forge

# List packages depending on `all-smi`:
mamba repoquery whoneeds all-smi --channel conda-forge

# List dependencies of `all-smi`:
mamba repoquery depends all-smi --channel conda-forge
```

</details>


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance,
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information, please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating all-smi-feedstock
==========================

If you would like to improve the all-smi recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/all-smi-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks, and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@pavelzw](https://github.com/pavelzw/)

