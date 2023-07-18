# fox-round-2
The repository for A Fox's Tale

## Working on tickets

    main    o---o----o---o---o----------o----o
                \    \                /    /
    feature1      \     o---o-----o--------o
                \                 /
    feature2        o---o------o---o

Main branch:
Represents our latest stable release. Should ONLY contain production-ready code.

Feature branch:
New code developed for any ticket. Is branched from `main`. Must be updated with `main` before creating a PR to merge back to `main` (ie. in this diagram, `feature2` must merge `main` into it to get `feature1` code and resolve any merge conflict before creating a PR).

## Branch Naming

Branch names will be of the following format: `PRODUCTCODE-ticketnumber-ticket-short-name`

Since we don't have a product name just yet, so for now we can do: `POC-01-setup-codebase`

## Commit Messages

The types `(feat/fix/doc)` will be used in the commit messages. The convention I personally use for those are
`type(feature being addressed): change summary + short rationale if applicable`
For instance:

1. `feat(fox movement): added horizontal movement`
2. `feat(fox horizontal movement): exposed movement speed for designers to tweak`
3. `fix(fox jump): forgot to lock z-axis`
4. `doc(convention): added commit message convention`
