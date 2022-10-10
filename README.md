# The calcite demonstrator API

The **calcite** demonstrator API is an **ArtifactDB** instance based on the [**gypsum** implementation](https://github.com/ArtifactDB/gypsum-worker).
It is customized to use a [different set of schemas](https://github.com/ArtifactDB/ExperimentHub-schemas) that enforces [ExperimentHub](https://bioconductor.org/packages/ExperimentHub)-like metadata standards.
In this repository, most of the customization involves editing [`wrangler.toml`](wrangler.toml) to point to a different R2 bucket;
we also use a [different CI/CD repository](https://github.com/ArtifactDB/calcite-actions), which is where the different schemas actually come into play.

Configuration of this fork was based on [these instructions](https://github.com/ArtifactDB/gypsum-worker#deployment-instructions).
