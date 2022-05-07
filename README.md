# Curated Package Collections for Idris2

This are package collections to be used with the
[*pack*](https://github.com/stefan-hoeck/idris2-pack) package manager
for Idris2.

In order to add your own package, make sure it builds with HEAD
of the main branch of the Idris2 project and submit a PR with
the package's description added to `collections/HEAD.toml`.

If it builds with Idris without failure, it will be included
in the next nightly release of the package collection. (At the
moment, collection's are checked semi-automatically and released
about once a day. Eventually we might have a different
release schedule).

Note about the `.db` files: These are from a very early version
of *pack* and are deprecated. I leave them here for the time
being but will eventually remove them.
