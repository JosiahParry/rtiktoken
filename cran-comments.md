Note for resubmit for version 0.0.6:

The following are fixed

- acronyms are now properly introduced (eg BPE, LLM)
- remove backticks in DESCRIPTION fields when referring to other languages/packages
- added more detailed description in DESCRIPTION

The following comments are given as well:

- the package does not use any webservice, all data (e.g., the encoders) are shipped with the package, therefore it functions completely offline. Hence we cannot add links to the DESCRIPTION fields for any webservice.
- there are no package installation calls in the part of the package that are used by the user. The only references to installations is in the Readme file (which shows how to install the package from CRAN, a chunk which is not executed), as well as in src/rust/vendor-authors.R, which is not called directly, instead it is a script to update the authors file from the rust packages in development mode. Note, I have added this script to .Rbuildignore just in case.
