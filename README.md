# Binder for BVCN Pseudo-Finder lesson

Initially forked from [here](https://github.com/binder-examples/conda). Thank you to the awesome [binder](https://mybinder.org/) team!

[![Binder](https://mybinder.org/badge_logo.svg)](https://gesis.mybinder.org/binder/v2/gh/Arkadiy-Garber/bvcn-binder-pseudofinder/master?urlpath=lab)

Part of the [Bioinformatics Virtual Coordination Network](https://biovcnet.github.io/) :)


## Walkthrough

Print general help menu

    pseudofinder.py help

Print the help menu of the Annotate module

    pseudofinder.py annotate -h

Run the Annotate module

    pseudofinder.py annotate -g test_data/Mycobacterium_leprae_TN.gbff -db test_data/combined_mycobacteria.faa -op testAnnotate

Print the help menu of the DNDS module

    pseudofinder.py dnds -h

Run the Annotate module

    pseudofinder.py dnds

Run the Annotate module, along with the DNDS module

    pseudofinder.py annotate




