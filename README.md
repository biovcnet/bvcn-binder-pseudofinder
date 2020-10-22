# Binder for BVCN Pseudo-Finder lesson

Initially forked from [here](https://github.com/binder-examples/conda). Thank you to the awesome [binder](https://mybinder.org/) team!

[![Binder](https://mybinder.org/badge_logo.svg)](https://gesis.mybinder.org/binder/v2/gh/biovcnet/bvcn-binder-pseudofinder/master?urlpath=lab)

Part of the [Bioinformatics Virtual Coordination Network](https://biovcnet.github.io/) :)

This module incorporates (wraps) several other programs/repositories, including

Pseudofinder
DIAMOND
PAML/codeml/pal2nal.pl
Muscle
BLAST


## Walkthrough

Print general help menu

    pseudofinder.py help

Print the help menu of the Annotate module

    pseudofinder.py annotate -h

Run the Annotate module

    pseudofinder.py annotate -g test_data/Mycobacterium_leprae_TN.gbff -db test_data/combined_mycobacteria.faa -op testAnnotate

Run the Annotate module, along with the DNDS module

    pseudofinder.py annotate -g test_data/Mycobacterium_leprae_TN.gbff -db test_data/combined_mycobacteria.faa -op testAnnotate --diamond -ref test_data/Mycobacterium_tuberculosis_H37Rv.gbff 

Print the help menu of the DNDS module

    pseudofinder.py dnds -h

Run the DNDS module

    pseudofinder.py dnds -a testAnnotate_proteome.faa -n testAnnotate_cds.fasta -ra testAnnotate_ref_proteome.faa -rn testAnnotate_ref_cds.fasta

