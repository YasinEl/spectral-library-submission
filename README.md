# Spectral library submission

A browser-only page for checking MS/MS spectra (`.mgf`, `.msp`, `.json`) before they are submitted to a
spectral library: https://yasinel.github.io/spectral-library-submission/

Files are parsed and checked in your browser; nothing is uploaded. **Submission is not connected yet**:
the Submit button builds the submission record and a receipt, but sends nothing.

The page checks structures (SMILES/InChI), adducts and precursor m/z, and asks for missing instrument and
acquisition metadata using PSI-MS and other ontology terms. Structures are checked with
[RDKit.js](https://github.com/rdkit/rdkit-js) (`RDKit_minimal.js` from jsDelivr, `RDKit_minimal.wasm` served here;
RDKit is BSD-3-Clause licensed).

This repository holds the built single-file page only.
