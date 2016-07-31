Following a [preliminary discussion](https://github.com/jpata/ROOT.jl/issues/4), 
we document the discussion the proposed julia API for ROOT.
This document is meant to be short and with code examples.
In the end, it should serve as a guide for ROOT users trying out julia.

# Object 
Anything derived from TObject and representing it in julia.

[discussion](https://github.com/jpata/API/issues/1)

* Where are the Cxx-side objects stored?
* When can julia gc collect a TObject?
* What to do with TObject::GetName()
* julia-side naming of ROOT classes.

# IO
TFile, TDirectory etc.

[discussion](https://github.com/jpata/API/issues/4)

* How to get rid of global file
* Semantics for writing objects to file
* Interface for TFile, TDirectory

# Tabular data
TTree, TChain related.

[discussion](https://github.com/jpata/API/issues/3)

* Interface for TTree, TChain 

# Histograms

* Interface for Histogram
* possibly Histogrammar.jl as the common backend: [discussion](https://github.com/jpata/API/pull/2)

# Misc

For each of these points, we can make issues where the discussion will be stored. Proposals can be PR-d into this document.
Let's keep it matter-of-fact and concise.
