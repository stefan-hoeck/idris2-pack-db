# Curated Package Collections for Idris2

[![Check Collection (ubuntu-latest)](https://github.com/stefan-hoeck/idris2-pack-db/actions/workflows/ci-db-ubuntu-latest.yml/badge.svg)](STATUS-ubuntu-latest.md)
[![Check Collection (macos-latest)](https://github.com/stefan-hoeck/idris2-pack-db/actions/workflows/ci-db-macos-latest.yml/badge.svg)](STATUS-macos-latest.md)

These are package collections to be used with the
[pack](https://github.com/stefan-hoeck/idris2-pack) package manager
for Idris2.

In order to add your own package, make sure it builds with HEAD
of the main branch of the Idris2 project and submit a PR with
the package's description added to `collections/HEAD.toml` and
make sure the necessary libraries are installed by adjusting
all six workflows under .github/workflows (there are two
variants of each workflow, one that runs on `ubuntu-latest`, and
one that runs on `macos-latest`).

As of [this](https://github.com/stefan-hoeck/idris2-pack/pull/417) PR,
`pack-admin` now looks at the `runsOn` field for every entry in
`collections/HEAD.toml`. If there is no `runsOn` field for a given
entry, then it is assumed that the given entry can build and test against
both `ubuntu` and `macos` platforms.

If it builds with Idris without failure, it will be included
in the next nightly release of the package collection. Nightly releases
are generated and checked automatically around 1 am UTC time
by a GitHub action on this repository.

You can see the current package list plus the build status of packages:
- Built and tested on ubuntu-latest [here](STATUS-ubuntu-latest.md).
- Built and tested on macos-latest [here](STATUS-macos-latest.md).
