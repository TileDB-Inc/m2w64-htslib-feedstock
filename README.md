About m2w64-htslib-feedstock
============================

Feedstock license: [BSD-3-Clause](https://github.com/TileDB-Inc/m2w64-htslib-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/samtools/htslib

Package license: MIT

Summary: C library for high-throughput sequencing data formats.

Development: https://github.com/TileDB-Inc/m2w64-htslib-build

Documentation: http://www.htslib.org/

The conda binary m2w64-htslib bundles a pre-built htslib binary that was
built under msys2. All dependencies are statically linked, with the
exception of .DLLs provided by Windows. It is suitable for linking against
in conda recipes that build using MSVC. It does not have libcurl support,
so cannot be used with S3 or GCS.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/TileDB-Inc/CI/_build/latest?definitionId=46&branchName=main">
            <img src="https://dev.azure.com/TileDB-Inc/CI/_apis/build/status/m2w64-htslib-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/TileDB-Inc/CI/_build/latest?definitionId=46&branchName=main">
                  <img src="https://dev.azure.com/TileDB-Inc/CI/_apis/build/status/m2w64-htslib-feedstock?branchName=main&jobName=win&configuration=win%20win_64_" alt="variant">
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
| [![Conda Recipe](https://img.shields.io/badge/recipe-m2w64--htslib-green.svg)](https://anaconda.org/tiledb/m2w64-htslib) | [![Conda Downloads](https://img.shields.io/conda/dn/tiledb/m2w64-htslib.svg)](https://anaconda.org/tiledb/m2w64-htslib) | [![Conda Version](https://img.shields.io/conda/vn/tiledb/m2w64-htslib.svg)](https://anaconda.org/tiledb/m2w64-htslib) | [![Conda Platforms](https://img.shields.io/conda/pn/tiledb/m2w64-htslib.svg)](https://anaconda.org/tiledb/m2w64-htslib) |

Installing m2w64-htslib
=======================

Installing `m2w64-htslib` from the `tiledb` channel can be achieved by adding `tiledb` to your channels with:

```
conda config --add channels tiledb
conda config --set channel_priority strict
```

Once the `tiledb` channel has been enabled, `m2w64-htslib` can be installed with `conda`:

```
conda install m2w64-htslib
```

or with `mamba`:

```
mamba install m2w64-htslib
```

It is possible to list all of the versions of `m2w64-htslib` available on your platform with `conda`:

```
conda search m2w64-htslib --channel tiledb
```

or with `mamba`:

```
mamba search m2w64-htslib --channel tiledb
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search m2w64-htslib --channel tiledb

# List packages depending on `m2w64-htslib`:
mamba repoquery whoneeds m2w64-htslib --channel tiledb

# List dependencies of `m2w64-htslib`:
mamba repoquery depends m2w64-htslib --channel tiledb
```




Updating m2w64-htslib-feedstock
===============================

If you would like to improve the m2w64-htslib recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`tiledb` channel, whereupon the built conda packages will be available for
everybody to install and use from the `tiledb` channel.
Note that all branches in the TileDB-Inc/m2w64-htslib-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@ihnorton](https://github.com/ihnorton/)
* [@jdblischak](https://github.com/jdblischak/)
* [@shelnutt2](https://github.com/shelnutt2/)
* [@teo-tsirpanis](https://github.com/teo-tsirpanis/)

