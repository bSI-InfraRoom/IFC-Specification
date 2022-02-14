The Increasing attribute is an optional attribute of the Pset_Stationing property set. It is meant for use in referents of predefined type REFERENCEMARKER being nested to a given alignment.

If present and true, or if not present, then the relevant subsequently nested STATION referents are expected to have Pset_Stationing.Station values being larger than the REFERENCEMARKER's Pset_Stationing.Station value.

If present and false, then the relevant subsequently nested STATION referents are expected to have Pset_Stationing.Station values being lower than the REFERENCEMARKER's Pset_Stationing.Station value.
