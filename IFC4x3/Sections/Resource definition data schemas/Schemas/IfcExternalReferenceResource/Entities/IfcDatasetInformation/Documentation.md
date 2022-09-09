_IfcDatasetInformation_ captures "metadata" of an external dataset. The actual content of the dataset is not defined in this specification; instead, it can be found following the _Location_ attribute.

The same _IfcDatasetInformation_ can be referenced from the exchange structure in total or in parts (e.g. by refering to particular chapters or paragraphs) using the _IfcDatasetReference_. All _IfcDatasetReference_'s that utilize the _IfcDatasetInformation_ are accessible by the inverse relationship _HasDatasetReferences_.
