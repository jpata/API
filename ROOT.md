Following a [preliminary discussion](https://github.com/jpata/ROOT.jl/issues/4), 
we document the discussion the proposed julia API for ROOT.
This document is meant to be short and with code examples.
In the end, it should serve as a guide for ROOT users trying out julia.

# Object
Anything derived from TObject and representing it in julia.

* Where are the Cxx-side objects stored?
* When can julia gc collect a TObject?
* Should TObject backed classes have a name (TObject::GetName)?

# IO
TFile, TDirectory etc.

* How to get rid of global file
* Semantics for writing objects to file
* Interface for TFile, TDirectory

# Tabular data
TTree, TChain related

* Interface for TTree, TChain

# Histograms

* Interface for Histogram

# Misc

For each of these points, we can make issues where the discussion will be stored. Proposals can be PR-d into this document.
Let's keep it matter-of-fact and concise.
