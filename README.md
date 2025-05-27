# IDN Spatial Data Catalogue

## Large Datasets
Datasets smaller than 100MB are in this repo, larger datasets are stored in IDN's OpenStack Swift object storage.

Update process - update date modified in manifest/metadata after updating dataset in OpenStack Swift

## Catalogue Resources

Resource | Role | Description
--- | --- | ---
Catalogue Definition:<br />[`catalogue.ttl`](catalogue.ttl) | [Catalogue Data](https://prez.dev/ManifestResourceRoles/CatalogueData) | The definition of, and medata for, the container which here is a dcat:Catalog object
Resource Data:<br />[`resources/*.nq`](resources/*.nq) | [Resource Data](https://prez.dev/ManifestResourceRoles/ResourceData) | dcat:Dataset objects in RDF (N-Quads) files in the resources/ folder
Profile Definition:<br />[`ogc_records_profile.ttl`](https://github.com/RDFLib/prez/blob/main/prez/reference_data/profiles/ogc_records_profile.ttl) | [Catalogue & Resource Model](https://prez.dev/ManifestResourceRoles/CatalogueAndResourceModel) | The default Prez profile for Records API
Labels:<br />[`_background/labels.ttl`](_background/labels.ttl) | [Incomplete Catalogue and Resource Labels](https://prez.dev/ManifestResourceRoles/IncompleteCatalogueAndResourceLabels) | An RDF file containing labels for catalogue's content, auto-extracted from KurrawongAI's Semantic Background
Manual Labels:<br />[`_background/labels-manual.ttl`](_background/labels-manual.ttl) | [Incomplete Catalogue and Resource Labels](https://prez.dev/ManifestResourceRoles/IncompleteCatalogueAndResourceLabels) | An RDF file containing labels for catalogue's content, manually created