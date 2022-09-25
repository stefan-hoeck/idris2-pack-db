# Curated Package Collections for Idris2

[![Check Collection](https://github.com/stefan-hoeck/idris2-pack-db/actions/workflows/ci-db.yml/badge.svg)](STATUS.md)

These are package collections to be used with the
[pack](https://github.com/stefan-hoeck/idris2-pack) package manager
for Idris2.

In order to add your own package, make sure it builds with HEAD
of the main branch of the Idris2 project and submit a PR with
the package's description added to `collections/HEAD.toml`.

If it builds with Idris without failure, it will be included
in the next nightly release of the package collection. Nightly releases
are generated and checked automatically around 1 am UTC time
by a GitHub action on this repository.

You can see the current package list plus the build status of
all packages [here](STATUS.md).
