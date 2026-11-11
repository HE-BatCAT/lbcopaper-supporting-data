# D1.3 metadata view as DCAT serialised as JSON-LD (from Zenodo)

The Zenodo folder has a verbatim mapping to a metadata file with a UUID. A DCAT serialised as JSON-LD 1.1 repecting folder structure, etc.
(any dataset collection would be a collection of IRIs made with these UUIDs)

This may be use to reference to any item within the uploaded deliverable (D1.3) or to add any further DCAT metadata at dataset/distribution level.

The files follow a SPDX path standard which is "relative to package". The SDPX distribution hash digest addition is now part of DCAT3.
Each file can be identified uniquely by its MD5 hash digest. All IDs and their corresponding IRIs are PIDs.

# Adding scientific data from partners

## Creating the Graph by weaving known scientific data
Here there is some draft metadata regarding the weaving of scientific data as a JSON-LD graph. 
There are some samples to understand the structure based on the content of a particular full cell.

(modelling from IFPEN data using LBCO, DVQ and QUDT so far)

./weaving/cells/
* *test-metadata.jsonld* is the reference working RDF document, so it is easy to growth with additions, possibly semi-automated, in both RDF and JSON mode.
* *test-metadata.n3* conversion to import on Protege.
* *test-cell.json* scratch pad file with example structure and IDs, kept for reference.


## Intended connection with the the DCAT metadata

Because this is based on the upload to Zenodo this is frozen. The template is based on may be upgraded (to update IRIs schemes, etc).
It will be the RDF reference connecting any files to other metadata (as long as not covered by DCAT).
Therefore, we may refer to a file with its corresponding hash digest and use that within the graph to connect further metadata.
The "@context" of JSON-LD may have provisions to convert plain identifiers into working IRIs.

* ./zenodo/D1.3_Repository/a4d5558c-cd40-4197-aa29-58643ba5c1e2.jsonld

WIP!
