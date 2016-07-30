Following a [preliminary discussion](https://github.com/jpata/ROOT.jl/issues/4), 
we document the discussion the proposed julia API for ROOT.
This document is meant to be short and with code examples.
In the end, it should serve as a guide for ROOT users trying out julia.

# Object
Anything derived from TObject and representing it in julia.

* Where are the Cxx-side objects stored? [Issue #1](https://github.com/JuliaHEP/API/issues/1)
* When can julia gc collect a TObject?
* What to do with TObject::GetName()
* julia-side naming of ROOT classes.

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
  * **Suggestion:** http://histogrammar.org/ (https://github.com/histogrammar/Histogrammar.jl); this is a platform-agnostic language for histograms that I'm in discussions with the ROOT team about integrating into ROOT. (Likely for PyROOT, maybe a C++ version for ROOT 7.) The Julia version of this interface would of course link into StatsBase.

# Misc

For each of these points, we can make issues where the discussion will be stored. Proposals can be PR-d into this document.
Let's keep it matter-of-fact and concise.
