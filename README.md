# chem2py
Find, convert, and use molecular properties and descriptors.

The vision here is a set of classes that abstract the idea that molecular entities are uniquely defined by their chemical structure, and thus knowing that structure, or any descriptor that maps to a single such structure, should serve as an index to *all* the publicly available data about that structure's properties. 

In practice, of course, it is often quite difficult to go from, say, a CDXML file of a chemical structure to, for example, knowing it's melting point. 

There are two principle reasons why it is difficult to access even the *publically available* information about chemical structures.

1. **There are multiple chemical descriptors that map to a single structure currently in common use.**
    SMILES amd Inchi, which can be used to recreate structure algorithmically but are very long and rarely used by humans,
    followed by the many database descriptors: CAS Number, PubChem ID, etc.,
    followed by structural information stored in various file-length formats such as MOL, SDF, PDB, or CDX / CDXML.
2. **There are multiple public sources of molecular properties currently in common use.**
    PubChem, ChemSpider, Wikipedia, various U.S. and other governmental agencies, and of course the primary literature, although much of that remains locked away from public use ([in theory](https://sci-hub.se)).

This project is a set of tools, written primarily in Python, intended to make it as simple as possible to know everything publically recorded about a given chemical structure, given ANY of the common identifiers which map to single chemical entities. 

## Thus, the overall goal: "All the molecular stuff in one place."
