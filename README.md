# kustomize-overlay-tag
Minimal example that attempts to set a new tag for a base image in a Kustomize overlay

To use:

    kustomize build ./overlays/dev
    kustomize build ./overlays/prd

Expected result:

* The `prd` overlay generates an image `eu.gcr.io/example-project/example-image:1.2.3`.
* The `dev` overlay generates an image `eu.gcr.io/example-project/example-image:1.2.3-SNAPSHOT`.
