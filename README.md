# Spack Contributions

This is a repo for the statistics we keep on the Spack project over time.
The repo contains [contrib](https://github.com/spack/contrib)
configuration files and a mapping from contributors to their
organizations, so that we can make a nice stacked area plot.

To generate the plots (note that this takes a while), run this:

```console
$ git clone https://github.com/spack/spack-contributions
$ cd spack-contributions
$ git submodule init
$ pip install -r requirements.txt
$ contrib
==> Indexing 49 commits.

STARTED       0/49 53ab298e88f80454f7f7c20ef200a3dbd0870473
    packages: processed 45/3487 blames (9.04/s)
...
```

You'll need [contrib](https://github.com/spack/contrib) installed and
`git` in your path.

This will generate plots of contributions to Spack's core, packages, and
documentation over time, based on Spack's git history.

To see the configuration that generates these plots, look at
[contrib.yaml](https://github.com/spack/spack-contributions/blob/master/contrib.yaml).
It has regexes that track the locations of different parts of the Spack
code over time.

## License

Spack is distributed under the terms of both the MIT license and the
Apache License (Version 2.0). Users may choose either license, at their
option.

All new contributions must be made under both the MIT and Apache-2.0
licenses.

See [LICENSE-MIT](https://github.com/spack/spack-contributions/blob/master/LICENSE-MIT),
[LICENSE-APACHE](https://github.com/spack/spack-contributions/blob/master/LICENSE-APACHE),
[COPYRIGHT](https://github.com/spack/spack-contributions/blob/master/COPYRIGHT), and
[NOTICE](https://github.com/spack/spack-contributions/blob/master/NOTICE) for details.

SPDX-License-Identifier: (Apache-2.0 OR MIT)

LLNL-CODE-811652
