## About ##
An exhaustive list of all Rust resources regarding automated or semi-automated formalization efforts in any area, constructive mathematics, formal algorithms, and program verification.

***As of May 29, 2022, proof of computation & cryptographic stuff are considered off-topic.***

awesome-rust-formalized-reasoning is an EDLA project.

The purpose of [edla.org](http://www.edla.org) is to promote the state of the art in various domains.


## Contents

- [Projects](#projects)
  - [Provers & Solvers](#provers-and-solvers)
    - [Provers TPTP compliant](#provers-tptp-compliant)
    - [SAT Solver](#sat-solver)
    - [Solver MPS compliant](#solver-mps-compliant)
    - [Proof assistant](#proof-assistant)
    - [Misc](#misc)
  - [Verification](#verification)
    - [Static Analysis & Rust verification tools](#static-analysis--rust-verification-tools)
    - [Misc](#misc-1)
  - [Libraries](#libraries)
    - [Parser](#parser)
    - [Bindings](#bindings)
    - [Translator](#translator)
    - [Misc](#misc-2)
  - [Books code](#books-code)
  - [Programming Language](#programming-language)
  - [Kanren](#kanren)
  - [Lambda Calculus](#lambda-calculus)
  - [Propositional Logic](#propositional-logic)
  - [Unclassified](#unclassified)
- [Resources](#resources)
  - [Books](#books)
  - [Crates keywords](#crates-keywords)
  - [Research Paper & Thesis](#research-paper--thesis)
  - [Demos](#demos)
  - [Blogs](#blogs)
  - [Posts](#posts)
  - [Community](#community)

---

## Legend

- Actively maintened :fire:
- Archived :skull:
- Benchmark :watch:
- Best in Class :diamonds:
- Book implementation :book:
- Crate(s) :package:
- Crates keyword fully listed :100:
- Deleted by author :recycle:
- Educational project :mortar_board:
- Exhumated :ghost:
- Inactive :zzz:
- List of resources :information_source:
- Paper with code :factory:
- Popular :star:
- Research paper :lab_coat:
- Toy project :baby_chick:
- Video :tv:
- WIP :construction:

## Projects

### Provers and Solvers

#### Provers TPTP compliant

- [CoP](https://github.com/01mf02/cop-rs) [:package:](https://crates.io/crates/cop) - reimplement automated theorem provers of the leanCoP family, such as leanCoP and nanoCoP.
- [lazyCoP](https://github.com/MichaelRawson/lazycop) [:watch:](https://www.tptp.org/CASC/J10/WWWFiles/DivisionSummary1.html):zzz: - automatic theorem prover for first-order logic with equality.
- [lerna](https://github.com/MichaelRawson/lerna) :skull: - proves theorems.
- [lickety](https://github.com/MichaelRawson/lickety) - prototype system for linear resolution with splitting.
- [meancop](https://github.com/01mf02/cop-rs) [:package:](https://crates.io/crates/meancop):recycle: - became CoP.
- [res-rs](https://github.com/philzook58/res-rs) :construction: - first bits for first-order logic prover.
- [Serkr](https://github.com/mAarnos/Serkr) :star:[:ghost:](https://github.com/newca12/Serkr) - automated theorem prover for first order logic with equality.
- [theorem-prover-rs](https://github.com/boitsov14/theorem-prover-rs) - rewrite of [theorem-prover-kt](https://github.com/boitsov14/theorem-prover-kt) a sequent-style automated theorem prover.

#### SAT Solver

- [backdoor-solver](https://github.com/Lipen/backdoor-solver) - backdoor-based SAT solver.
- [BatSat](https://github.com/c-cube/batsat) [:package:](https://crates.io/crates/batsat):star: - solver forked from ratsat, a reimplementation of MiniSat.
- [Colombini-SAT](https://github.com/Lorenzinco/colombiniSAT) - simple 3-SAT solver.
- [CreuSAT](https://github.com/sarsko/CreuSAT) :star: - formally verified SAT solver verified with Creusot.
- [Debug-SAT](https://github.com/advancedresearch/debug_sat) [:package:](https://crates.io/crates/debug_sat) - debuggable automatic theorem prover for boolean satisfiability problems (SAT).
- [dpll-sat](https://github.com/snsinfu/dpll-sat) :zzz: - naïve SAT solver implementing the classic DPLL algorithm.
- [DRSAT](https://github.com/danielschemmel/drsat) - Daniel's Rusty SAT solver.
- [lutrix](https://github.com/arata-nvm/lutrix) :zzz: - SAT/SMT Solver.
- [microsat](https://github.com/RobScheidegger/microsat) [:package:](https://crates.io/crates/microsat) - tiny DPLL SAT-solver.
- [minisat-rust](https://github.com/mishun/minisat-rust) :star::zzz: - experimental minisat SAT solver.
- [msat](https://github.com/solhop/msat) [:package:](https://crates.io/crates/msat):skull: - MaxSAT Solver.
- [RatSat](https://github.com/qnighy/ratsat) [:package:](https://crates.io/crates/ratsat)[:package:](https://crates.io/crates/ratsat-bin):star::zzz: - reimplementation of MiniSat.
- [Resolvo](https://github.com/mamba-org/resolvo) [:package:](https://crates.io/crates/resolvo):star: - fast package resolver (CDCL based SAT solving).
- [rsat](https://github.com/solhop/rsat) [:package:](https://crates.io/crates/rsat):skull: - SAT Solver.
- [RsBDD](https://github.com/timbeurskens/rsbdd) - Reduced-order Binary Decision Diagram (RoBDD) SAT solver.
- [rust-sat](https://github.com/michaelbeaumont/rust-sat) :zzz: - SAT solver that accepts input in the DIMACS CNF file format.
- [rustsat(2)](https://github.com/jamesbornholt/rustsat) :baby_chick: - toy SAT solver.
- [sat](https://github.com/KomaEc/sat) - simple CDCL sat solver.
- [SAT solver](https://github.com/shinkwhek/SATsolver) :baby_chick::zzz: - SAT solver.
- [SAT Solver(2)](https://github.com/NVictor2004/SATSolver) :baby_chick: - simple SAT solver.
- [SAT-MICRO](https://github.com/OCamlPro/sat_micro_rust) [:lab_coat:](https://hal.inria.fr/inria-00202831/en) - reimplementation of the SAT-solver described in 'SAT-MICRO: petit mais costaud!'.
- [sat-solver](https://github.com/RobertObkircher/sat-solver) - simple CDCL SAT solver based on the lecture 185.A93 Formal Methods in CS at TU Wien.
- [SAT-Solver](https://github.com/FWuermse/SAT-Solver) - DPLL and CDCL Solver.
- [SATCoP](https://github.com/MichaelRawson/satcop) :zzz: - theorem prover for first-order logic based on connection tableau and SAT solving.
- [Satire](https://github.com/Qwaz/satire) [:package:](https://crates.io/crates/satire):zzz: - educational SAT solver.
- [satyrs](https://github.com/jayelm/satyrs) :mortar_board::zzz: - DPLL SAT solver.
- [scrapsat](https://github.com/togatoga/scrapsat) :zzz: - CDCDL SAT Solver.
- [screwsat](https://github.com/togatoga/screwsat) [:package:](https://crates.io/crates/screwsat):star: - simple CDCL SAT Solver.
- [Scuttle](https://github.com/chrjabs/scuttle) [:package:](https://crates.io/crates/scuttle)[:package:](https://crates.io/crates/scuttle-proc) - multi-objective MaxSAT solver based on the rustsat library and the CaDiCaL SAT solver.
- [simple-sat](https://github.com/sidorov-ks/simple-sat) - one of the SAT solvers of all time.
- [~~slp~~](https://github.com/solhop/slp) [:package:](https://crates.io/crates/slp):recycle: - became SolHOP.
- [SolHOP](https://github.com/solhop/solhop) [:package:](https://crates.io/crates/solhop):skull: - aims to be a SAT and MaxSAT solver. Currently, a CDCL based SAT.
- [Splr](https://github.com/shnarazk/splr) [:package:](https://crates.io/crates/splr):diamonds::star: - modern CDCL SAT solver.
- [starlit](https://github.com/jix/starlit) :construction: - CDCL SAT solver.
- [Stevia](https://github.com/Robbepop/stevia) :star::zzz: - simple (unfinished) SMT solver for QF_ABV.
- [UASAT-RS](https://github.com/mmaroti/uasat-rs) - SAT solver based calculator for discrete mathematics and universal algebra.
- [Varisat](https://github.com/jix/varisat)[:package:](https://crates.io/crates/varisat)[:package:](https://crates.io/crates/varisat-checker)[:package:](https://crates.io/crates/varisat-cli)[:package:](https://crates.io/crates/varisat-dimacs)[:package:](https://crates.io/crates/varisat-formula)[:package:](https://crates.io/crates/varisat-internal-macros)[:package:](https://crates.io/crates/varisat-internal-proof)[:package:](https://crates.io/crates/varisat-lrat):star: - CDCL based SAT solver.

#### Solver MPS compliant

- [ellp](https://github.com/kehlert/ellp) [:package:](https://crates.io/crates/ellp):construction: - linear programming library that provides primal and dual simplex solvers.
- [microlp](https://github.com/Specy/microlp) [:package:](https://crates.io/crates/microlp) - linear programming solver (fork of [minilp](https://github.com/ztlpn/minilp)).
- [minilp](https://github.com/ztlpn/minilp) [:package:](https://crates.io/crates/minilp):star::skull: - linear programming solver.

#### Proof assistant

- [hakim](https://github.com/babaeee/hakim) - hacky interactive theorem prover.
- [~~cobalt~~](https://github.com/lcnr/cobalt) :recycle:[:ghost:](https://github.com/isgasho/cobalt) - a wip minimal proof assistant.
- [Esther](https://github.com/aodhneine/esther) :zzz: - simple automated proof assistant.
- [homotopy-rs](https://github.com/homotopy-io/homotopy-rs) [:lab_coat:](https://arxiv.org/abs/1812.10586)[:lab_coat:](https://arxiv.org/abs/1902.03831):diamonds::star: - implementation of homotopy.io proof assistant.
- [LSTS](https://github.com/andrew-johnson-4/LSTS) [:package:](https://crates.io/crates/lsts):star: - proof assistant that is also a programming language.
- [Noq](https://github.com/tsoding/Noq) [:tv:](https://www.youtube.com/playlist?list=PLpM-Dvs8t0VZVE64QKPf6y_TIUwj5nKQ7):star: - Not Coq. Simple expression transformer that is not Coq.
- [minimo](https://github.com/gpoesia/minimo) [:lab_coat:](https://arxiv.org/abs/2407.00695)[:lab_coat:](https://arxiv.org/abs/2211.15864):diamonds::star: - An environment for learning formal mathematical reasoning from scratch.
- [Poi](https://github.com/advancedresearch/poi) [:package:](https://crates.io/crates/poi):star: - pragmatic point-free theorem prover assistant.
- [Proost](https://gitlab.crans.org/loutr/proost) - simple proof assistant.
- [qbar](https://github.com/qdeduction/qbar) [:package:](https://crates.io/crates/qbar):zzz: - experimental automated theorem verifier/prover and proof assistant.

#### Misc

- [Avalog](https://github.com/advancedresearch/avalog) [:package:](https://crates.io/crates/avalog):star: - experimental implementation of Avatar Logic with a Prolog-like syntax.
- [autosat](https://github.com/petersn/autosat-rs) [:package:](https://crates.io/crates/autosat):baby_chick: - automatic conversion of functions to CNF for SAT solving.
- [bootfrost](https://github.com/snigavik/bootfrost) - automated theorem proving program for first-order formulas with extensions.
- [Caso](https://github.com/advancedresearch/caso) [:package:](https://crates.io/crates/caso) - category Theory Solver for Commutative Diagrams.
- [cyclegg](https://github.com/nadia-polikarpova/cyclegg):star: - cyclic theorem prover for equational reasoning using egraph.
- [good_lp](https://github.com/rust-or/good_lp) :star: - Mixed Integer Linear Programming modeler using external solvers.
- [gpp-solver](https://github.com/Ereski/gpp-solver) [:package:](https://crates.io/crates/gpp-solver) - small hybrid push-pull solver/planner that has the best of both worlds.
- [hoice](https://github.com/hopv/hoice) :star: - ICE-based Constrained Horn Clause (CHC) solver.
- [linear_solver](https://github.com/advancedresearch/linear_solver) [:package:](https://crates.io/crates/linear_solver):star: - linear solver designed to be easy to use with Rust enums.
- [Logic solver](https://github.com/qnighy/logic-solver-rs) :star::zzz: - logic solver.
- [Mikino](https://github.com/OCamlPro/mikino) [:package:](https://crates.io/crates/mikino)[:package:](https://crates.io/crates/mikino_api) - simple induction and BMC engine.
- [Monotonic-Solver](https://github.com/advancedresearch/monotonic_solver) [:package:](https://crates.io/crates/monotonic_solver):star: - monotonic solver designed to be easy to use with Rust enum expressions.
- [nnoq](https://github.com/pro465/nnoq) - simple theorem prover (nay, verifier) based on functional expression rewriting.
- [nyaya](https://github.com/pro465/nyaya) - proof language based on [sequent calculus](https://en.wikipedia.org/wiki/Sequent_calculus) and [Metamath](https://us.metamath.org).
- [Obvious](https://github.com/hargoniX/obvious) :zzz: - simple little logic solver and calculator.
- [pocket_prover](https://github.com/advancedresearch/pocket_prover) [:package:](https://crates.io/crates/pocket_prover)[:package:](https://crates.io/crates/pocket_prover-derive):star: - fast, brute force, automatic theorem prover for first order logic.
- [prover](https://github.com/varqox/prover) :skull: - first-order logic prover.
- [prover(2)](https://github.com/mverleg/prover) :baby_chick::zzz: - experiment with integer relation prover.
- [QED Prover](https://github.com/qed-solver/prover) :star:[:lab_coat:](https://www.vldb.org/pvldb/vol11/p1482-chu.pdf) - reimplementation of the Cosette prover in Rust.
- [reachability_solver](https://github.com/advancedresearch/reachability_solver) [:package:](https://crates.io/crates/reachability_solver) - linear reachability solver for directional edges.
- [relsat-rs](https://github.com/mmaroti/relsat-rs) :baby_chick: - Experiments with  provers.
- [SAT-bench](https://github.com/shnarazk/SAT-bench) - benchmark suit for SAT solvers.
- [sat_lab](https://github.com/arenaudineau/sat_lab) :baby_chick::construction: - framework for manipulating SAT problems.
- [SAT solver ANalyser](https://github.com/SAT-solver-ANalyzer/SATAn) :construction: - toolbox for analyzing performance and runtime characteristics of SAT solvers.
- [sequentprover](https://github.com/astrobeastie/sequentprover) :baby_chick: - proof search algorithm for boolean formulae.
- [Sequent solver](https://github.com/Dacit/sequent_prover) :baby_chick::zzz: - simple sequent solver.
- [shari](https://github.com/nyuichi/shari) - the 🍣 prover.
- [stupid-smt](https://github.com/Hoblovski/stupid-smt) :baby_chick::zzz: - SMT library. Mainly project at the verification course in THU.
- [Tensor Theorem Prover](https://github.com/chanind/tensor-theorem-prover) - first-order logic theorem prover (support unification with approximate vector similarity).
- [theorem-prover](https://github.com/jchenche/theorem-prover) - implementation of a theorem prover for first-order logic.
- [Totsu](https://github.com/convexbrain/Totsu) [:package:](https://crates.io/crates/totsu)[:package:](https://crates.io/crates/totsu_f32cuda)[:package:](https://crates.io/crates/totsu_f64lapack)[:package:](https://crates.io/crates/totsu_core)[:package:]():star: - first-order conic solver for convex optimization problems .

### Verification

#### Static Analysis & Rust verification tools/framework

- [Charon](https://github.com/sonmarcho/charon) :star:[:lab_coat:](https://arxiv.org/abs/2410.18042):fire: - interface with the rustc compiler for the purpose of program verification.
- [coq-of-rust](https://github.com/formal-land/coq-of-rust) :star: - formal verification for Rust.
- [contracts](https://gitlab.com/karroffel/contracts) [:package:](https://crates.io/crates/contracts):star: - implements "[Design By Contract](https://en.wikipedia.org/wiki/Design_by_contract)" via procedural macros.
- [Creusot](https://github.com/xldenis/creusot) :star::fire: - tool for deductive verification of Rust code.
- [crux-mir](https://github.com/GaloisInc/crucible/tree/master/crux-mir) :star:[:lab_coat:](https://arxiv.org/abs/2410.18280) - static simulator for Rust programs.
- [cwe_checker](https://github.com/fkie-cad/cwe_checker) :star: - finds vulnerable patterns in binary executables.
- [electrolysis](https://github.com/Kha/electrolysis) :star::zzz: - tool for formally verifying Rust programs by transpiling them into the Lean 2 theorem prover.
- [Flux](https://github.com/flux-rs/flux) [:tv:](https://www.youtube.com/watch?v=k-izcFCHN2o):star:[:lab_coat:](https://arxiv.org/pdf/2207.04034.pdf):fire: - refinement type checker for Rust.
- [Granite](https://github.com/Skasselbard/Granite) :star:[:lab_coat:](https://github.com/Skasselbard/Granite/blob/master/doc/MasterThesis/main.pdf):zzz: - find Deadlocks in Rust with Petri-Net Model checking.
- [Kani](https://github.com/model-checking/kani) [:package:](https://crates.io/crates/kani-verifier):star:[:lab_coat:](https://www.cs.cornell.edu/~avh/dyn-trait-icse-seip-2022-preprint.pdf):fire: - bit-precise model-checker, ensures that unsafe Rust code is actually safe.
- [Liquid Rust](https://github.com/fan-tom/liquid-rust) :star::zzz: - implement Liquid Types type checker.
- [lockbud](https://github.com/BurtonQin/lockbud) :star:[:lab_coat:](https://songlh.github.io/paper/rust-study.pdf) - statically detect deadlocks bugs for Rust.
- [Logically Qualified Data Types](https://github.com/bpowers/liquid-types) - implementation of liquid types on an implicitly-typed variant of ML.
- [Loom](https://github.com/tokio-rs/loom) [:package:](https://crates.io/crates/loom):star: - concurrency permutation testing tool for Rust.
- [matla](https://github.com/OCamlPro/matla) - a manager for TLA+ projects.
- [MIRAI](https://github.com/facebookexperimental/MIRAI) [:package:](https://crates.io/crates/mirai-annotations):star: - intended to become a widely used static analysis tool for Rust.
- [MirChecker](https://github.com/lizhuohua/rust-mir-checker) :star:[:lab_coat:](https://www.cse.cuhk.edu.hk/~cslui/PUBLICATION/CCS2021.pdf) - simple static analysis tool.
- [p4-analyzer](https://github.com/AzureMarker/p4-analyzer) - static analysis tool which checks P4 code for bugs.
- [Prusti](https://github.com/viperproject/prusti-dev) [:package:](https://crates.io/crates/prusti-contracts)[:package:](https://crates.io/crates/prusti-contracts-proc-macros)[:package:](https://crates.io/crates/prusti-specs)[:package:](https://crates.io/crates/prusti-std):star::fire: - prototype verifier for Rust, built upon the the Viper verification infrastructure.
- [RefinedRust](https://gitlab.mpi-sws.org/lgaeher/refinedrust-dev) [:lab_coat:](https://dl.acm.org/doi/10.1145/3656422) - type system for high-assurance verification of Rust Programs.
- [Rudra](https://github.com/sslab-gatech/Rudra) :star:[:lab_coat:](https://github.com/sslab-gatech/Rudra/blob/master/rudra-sosp21.pdf) - static analyzer to detect common undefined behaviors in Rust programs.
- [Rust Software Verification Benchmarks](https://github.com/alastairreid/rust-benchmarks) :zzz: - collection of Rust verification benchmarks with their verifier crates.
- [Rust static analysis/verification reading and resources](https://github.com/facebookexperimental/MIRAI/blob/main/documentation/FurtherReading.md) :information_source: - for further reading.
- [Rust verification tools](https://github.com/project-oak/rust-verification-tools) :star: - collection of tools/libraries about static and dynamic verification of Rust programs.
- [Rust verification tools (2021)](https://rust-formal-methods.github.io/tools.html) :information_source: - list of Rust verification tools with a bias towards ‘formal methods’ tools.
- [Rust verification tools list](https://alastairreid.github.io/automatic-rust-verification-tools-2021) :information_source: - list of tools.
- [RustHorn](https://github.com/hopv/rust-horn) :star:[:lab_coat:](https://link.springer.com/chapter/10.1007%2F978-3-030-44914-8_18) - CHC-based Automated Verification Tool for Rust.
- [RustHornBelt Library & Benchmarks](https://github.com/xldenis/rhb-specs) [:lab_coat:](https://zenodo.org/record/6426048) - evaluation libraries and benchmarks for the RustHornBelt PLDI paper.
- [Rustproof](https://github.com/Rust-Proof/rustproof) [:package:](https://crates.io/crates/rustproof):star::zzz: - compiler plugin, verification condition generator.
- [Shuttle](https://github.com/awslabs/shuttle) [:package:](https://crates.io/crates/shuttle):star: - library for testing concurrent Rust code.
- [Stateright](https://github.com/stateright/stateright) [:package:](https://crates.io/crates/stateright):star: - model checker for implementing distributed systems.
- [VeriWasm](https://github.com/PLSysSec/veriwasm) [:package:](https://crates.io/crates/veriwasm):star:[:lab_coat:](http://cseweb.ucsd.edu/~dstefan/pubs/johnson:2021:veriwasm.pdf) - SFI verifier of Wasm binaries.
- [verus](https://github.com/secure-foundations/verus) :star::fire:[:tv:](https://www.youtube.com/watch?v=ZZTk-zS4ZCY)[:lab_coat:](https://arxiv.org/abs/2303.05491) - verified subset of Rust for low-level systems code.
- [Xori](https://github.com/endgameinc/xori) :star::zzz: - static analysis library for PE32, 32+ and shellcode.

#### Misc

- [ArcsJs - Provable](https://github.com/project-oak/arcsjs-provable) - set of ArcsJs focused tools for doing proofs on ArcsJs models.
- [Bounded Registers](https://github.com/auxoncorp/bounded-registers) [:package:](https://crates.io/crates/bounded-registers):star: - high-assurance memory-mapped register interaction library.
- [Carcara](https://github.com/ufmg-smite/carcara) :star:[:lab_coat:](https://team.inria.fr/veridis/files/2023/05/carcara.pdf) - proof checker and elaborator for SMT proofs in the [Alethe format](https://verit.gitlabpages.uliege.be/alethe/specification.pdf).
- [ceetle](https://github.com/AzeezDa/ceetle) [:package:](https://crates.io/crates/ceetle)[:package:](https://crates.io/crates/ceetle_macros) - library for defining models in Computational Tree Logic and verifying their semantics.
- [Chalk](https://github.com/rust-lang/chalk) [:package:](https://crates.io/crates/chalk-solve)[:package:](https://crates.io/crates/chalk-derive)[:package:](https://crates.io/crates/chalk-engine)[:package:](https://crates.io/crates/chalk-ir)[:package:](https://crates.io/crates/chalk-macros)[:package:](https://crates.io/crates/chalk-recursive)[:package:](https://crates.io/crates/chalk-rust-ir):star: - implements the Rust trait system, based on Prolog-ish logic rules.
- [Kinō](https://github.com/kino-mc/kino) :skull: - re-implementation of the core verification engine of [Kind 2 model-checker](https://kind2-mc.github.io/kind2).
- [Kontroli](https://github.com/01mf02/kontroli-rs) [:package:](https://crates.io/crates/dedukti-parse)[:package:](https://crates.io/crates/kocheck)[:package:](https://crates.io/crates/kontroli):star::diamonds:[:tv:](https://www.youtube.com/watch?v=lLjWBsU_BX0)[:lab_coat:](https://arxiv.org/pdf/2102.08766.pdf) - alternative implementation of the logical framework Dedukti.
- [Metamath-knife](https://github.com/metamath/metamath-knife) [:package:](https://crates.io/crates/metamath-rs):star:  - verify Metamath proofs.
- [Mist](https://github.com/oeb25/mist) - userfriendly verification frontend language.
- [Mizar proof checker](https://github.com/digama0/mizar-rs) :star::construction: - Alternative [Mizar](http://mizar.org) proof checker.
- [pocket_prover-set](https://github.com/advancedresearch/pocket_prover-set) [:package:](https://crates.io/crates/pocket_prover-set) - base logical system for PocketProver to reason about set properties.
- [rate](https://github.com/krobelus/rate) [:package:](https://crates.io/crates/rate)[:package:](https://crates.io/crates/rate-common)[:package:](https://github.com/krobelus/rate)[:package:](https://crates.io/crates/rate-proof-utils)[:package:](https://crates.io/crates/rate-sick-check):diamonds:[:lab_coat:](https://github.com/krobelus/rate-experiments/blob/master/thesis.pdf) - clausal proof checker (DRAT, DPR) for certifying SAT solvers' unsatisfiability results.
- [rlfsc](https://github.com/alex-ozdemir/rlfsc) [:package:](https://crates.io/crates/rlfsc):zzz: - checker for the LFSC proof language.
- [second_opinion](https://github.com/ammkrn/second_opinion) - verifier for Metamath Zero proof files.
- [smetamath](https://github.com/sorear/smetamath-rs) [:package:](https://crates.io/crates/smetamath):star::zzz: - parallel and incremental verifier for Metamath databases.
- [Supervisionary](https://github.com/DominicPM/supervisionary) [:tv:](https://www.youtube.com/watch?v=4iOTl-XowAo)[:lab_coat:](https://dominicpm.github.io/publications/mulligan-supervisionary-2022.pdf) - experimental proof-checking system for Gordon's higher-order logic.
- [t3p](https://github.com/skbaek/tesc/tree/master/t3p-rs) - optimized TESC (Theory-Extensible Sequent Calculus) verifier.
- [Temporal Verifier](https://github.com/vmware-research/temporal-verifier) :star: - framework for temporal verification based on first-order linear-time temporal logic.
- [verifiable-controllers](https://github.com/vmware-research/verifiable-controllers) :star: - framework to build practical, formally verified, cluster management controllers.
- [Verifier](https://github.com/trivial-rs/verifier) [:package:](https://crates.io/crates/trivial-verifier):zzz: - Trivial proof verifier - an interface to the Metamath Zero kernel.

### Libraries

#### Parser

- [CNF Parser](https://github.com/robbepop/cnf-parser) [:package:](https://crates.io/crates/cnf-parser):zzz: - efficient and customizable parser for the .cnf file format.
- [coq-rs](https://github.com/digama0/coq-rs) - this program can parse Coq .vo files.
- [DIMACS Parser](https://github.com/robbepop/dimacs-parser) [:package:](https://crates.io/crates/dimacs) - utilities to parse files in DIMACS .cnf or .sat file format.
- [Exec-SAT](https://github.com/matszpk/exec-sat) [:package:](https://crates.io/crates/exec-sat):baby_chick: - provides routines to parse SAT solver output and to execute SAT solver.
- [Flussab CNF](https://github.com/jix/flussab) [:package:](https://crates.io/crates/flussab-cnf) - parsing and writing of the DIMACS CNF file format.
- [FRAT-rs](https://github.com/digama0/frat) [:lab_coat:](https://arxiv.org/pdf/2109.09665.pdf) - toolchain for processing and transforming files in the FRAT format.
- [isabelle export tool](https://github.com/digama0/isabelle-rs) - parser for isabelle database files.
- [Lambda Calculus Parser](https://github.com/notJoon/lambda) - λ-calculus parser.
- [Lambda Term Parsing](https://github.com/01mf02/lambda-parse) - explores different parser designs for a simple lambda term grammar.
- [logic-form](https://github.com/gipsyh/logic-form) [:package:](https://crates.io/crates/logic-form):baby_chick: - library for representing Cube, Clause, CNF and DNF.
- [logic-parser](https://github.com/paoloose/discrete-mathematics/tree/main/assignments/week1/logic-parser) [:package:](https://crates.io/crates/logic-parser):mortar_board: - library for lexing, parsing and visualizing logical expressions.
- [lp_parser_rs](https://github.com/dandxy89/lp_parser_rs) [:package:](https://crates.io/crates/lp_parser_rs) - LP file parser.
- [mmb-parser](https://github.com/trivial-rs/mmb-parser) [:package:](https://crates.io/crates/mmb-parser) - parser for the Metamath Zero binary proof format.
- [mps](https://github.com/integrated-reasoning/mps) [:package:](https://crates.io/crates/mps) - fast MPS parser.
- [olean-rs](https://github.com/digama0/olean-rs) :zzz: - parser/viewer for olean files.
- [Patronus](https://github.com/ekiwi/patronus) [:package:](https://crates.io/crates/patronus):construction: - btor2 parser, wip hardware bug-finding toolkit.
- [RustLogic](https://github.com/Rose1917/rustlogic) [:package:](https://crates.io/crates/rustlogic-march1917) - parsing and handling simple logical expressings.
- [smt2](https://github.com/regular-pv/smt2) [:package:](https://crates.io/crates/smt2) - SMT-LIB 2 parsing library.
- [tptp](https://github.com/MichaelRawson/tptp) [:package:](https://crates.io/crates/tptp):diamonds: - parse the TPTP format.

#### Bindings

- [boolector](https://github.com/cdisselkoen/boolector-rs) [:package:](https://crates.io/crates/boolector) - safe high-level bindings for the [Boolector](https://boolector.github.io) SMT solver.
- [bitwuzla-sys](https://github.com/fatemender/bitwuzla-sys) [:package:](https://crates.io/crates/bitwuzla-sys) - low-level bindings for the [Bitwuzla](https://bitwuzla.github.io) SMT solver.
- [boolector-sys](https://github.com/fatemender/boolector-sys) [:package:](https://crates.io/crates/boolector-sys) - low-level bindings for the [Boolector](https://boolector.github.io) SMT solver.
- [cadical-rs](https://github.com/mmaroti/cadical-rs) [:package:](https://crates.io/crates/cadical) - bindings for the CaDiCaL SAT solver.
- [cat_solver](https://github.com/UncombedCoconut/cat_solver) [:package:](https://crates.io/crates/cat_solver) - bindings for the Kissat SAT solver.
- [clingo-rs](https://github.com/potassco/clingo-rs) [:package:](https://crates.io/crates/clingo)[:package:](https://crates.io/crates/clingo-derive)[:package:](https://crates.io/crates/clingo-sys):star: - idiomatic bindings to the [clingo](https://github.com/potassco/clingo) library.
- [cplex-rs](https://github.com/mbiggio/cplex-rs) [:package:](https://crates.io/crates/cplex-rs)[:package:](https://crates.io/crates/cplex-rs-sys) - safe rust bindings for [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer).
- [cryptominisat-rs](https://github.com/storyyeller/cryptominisat-rs) [:package:](https://crates.io/crates/cryptominisat):zzz: - bindings for [CryptoMiniSat](https://github.com/msoos/cryptominisat).
- [falcon-z3](https://github.com/falconre/falcon-z3) [:package:](https://crates.io/crates/falcon-z3) - bindings for Z3.
- [highs](https://github.com/rust-or/highs) [:package:](https://crates.io/crates/highs) - safe rust bindings for the [HiGHS](https://highs.dev) linear programming solver.
- [highs-sys](https://github.com/rust-or/highs-sys) [:package:](https://crates.io/crates/highs-sys) - bindings for the [HiGHS](https://highs.dev) linear programming solver.
- [IPASIR](https://github.com/robbepop/ipasir-rs) [:package:](https://crates.io/crates/ipasir):zzz: - FFI bindings for the IPASIR incremental SAT solver interface.
- [Ipasir-loading]() [:package:](https://crates.io/crates/ipasir-loading) - load shared libraries of IPASIR compatible SAT solvers.
- [isabelle-client](https://github.com/lotzk/rust-isabelle-client) [:package:](https://crates.io/crates/isabelle-client) - client to interact with an [Isabelle](https://isabelle.in.tum.de) server.
- [Kissat-rs](https://github.com/firefighterduck/kissat-rs) [:package:](https://crates.io/crates/kissat) - bindings for the Kissat SAT solver.
- [lean-sys](https://gitlab.com/tekne/lean-sys) [:package:](https://crates.io/crates/lean-sys) - bindings to Lean 4's C API.
- [libsmt.rs](https://github.com/sushant94/libsmt.rs) :zzz: - bindings for SMTLIB2.
- [logicng-open-wbo-sys](https://github.com/booleworks/logicng-rs) [:package:](https://crates.io/crates/logicng-open-wbo-sys) - low-level LogicNG bindings for the MaxSAT solver [Open-WBO](https://github.com/sat-group/open-wbo).
- [lpsolve](https://docs.rs/crate/lpsolve/latest/source) [:package:](https://crates.io/crates/lpsolve)[:package:](https://crates.io/crates/lpsolve-sys):zzz: - high-level [lpsolve](https://sourceforge.net/projects/lpsolve) wrapper.
- [maxpre-rs](https://github.com/chrjabs/maxpre-rs) [:package:](https://crates.io/crates/maxpre) - bindings for the (multi-objective) MaxSAT preprocessor MaxPre.
- [pblib-rs](https://github.com/crillab/pblib-rs) [:package:](https://crates.io/crates/pblib-rs) - safe bindings for [pblib](https://github.com/master-keying/pblib).
- [rplex](https://github.com/emallson/rplex) :zzz: - bindings for [CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio/cplex-optimizer).
- [rsmt2](https://github.com/kino-mc/rsmt2) [:package:](https://crates.io/crates/rsmt2)[:package:](https://crates.io/crates/rsmt2-zz):star: - generic library to interact with SMT-LIB 2 compliant solvers.
- [rssat](https://github.com/francisol/rssat) [:package:](https://crates.io/crates/rssat) - provides Rust bindings for multiple popular SAT solvers.
- [russcip](https://github.com/scipopt/russcip) [:package:](https://crates.io/crates/russcip):star: - safe Rust interface for [SCIP](https://www.scipopt.org).
- [Rust-SMT-LIB-API](https://github.com/facebookarchive/Rust-SMT-LIB-API) [:package:](https://crates.io/crates/rust_smt):star::skull: - generic high-level API for interacting with SMT solvers.
- [rust_z3prover](https://github.com/hrkzmnm/rust_z3prover) :zzz: - use Z3 SMT solver from rust.
- [rustproof-libsmt](https://github.com/Rust-Proof/libsmt.rs) [:package:](https://crates.io/crates/rustproof-libsmt):zzz: - fork of libsmt.rs.
- [SAT Nexus](https://github.com/Lipen/sat-nexus) - interfaces and wrappers for SAT solvers.
- [scip-sys](https://github.com/scipopt/scip-sys) [:package:](https://crates.io/crates/scip-sys) - raw rust bindings to [SCIP](https://www.scipopt.org).
- [smt_sb-rs](https://github.com/DavidD12/smt_sb-rs) [:package:](https://crates.io/crates/smt_sb-rs) - Z3 SMT Simple Binding.
- [smtlib](https://github.com/oeb25/smtlib-rs) [:package:](https://crates.io/crates/smtlib)[:package:](https://crates.io/crates/smtlib-lowlevel)[:package:](https://crates.io/crates/smtlib-build-util) - high-level API for interacting with SMT solvers.
- [vipers](https://github.com/oeb25/vipers) - crates for interacting with the Viper verification infrastructure.
- [Yices2](https://github.com/novafacing/yices2-rs) [:package:](https://crates.io/crates/yices2)[:package:](https://crates.io/crates/yices2-sys) - low and high-level bindings to the [Yices2](https://yices.csl.sri.com/) SMT solver.
- [z3](https://github.com/prove-rs/z3.rs) [:package:](https://crates.io/crates/z3)[:package:](https://crates.io/crates/z3-sys):star::fire: - high-level and low-level Rust bindings for the Z3 solver.
- [z3-rust](https://github.com/p4l1ly/z3-rust) [:package:](https://crates.io/crates/z3_ref) :zzz: - high level bindings for the Microsoft's Z3 SMT solver.
- [Z3D](https://github.com/alex-chew/z3d-rs) [:package:](https://crates.io/crates/z3d):zzz: - Z3 DSL interface.

#### Translator

- [anthem](https://github.com/potassco/anthem) :zzz: - translate answer set programs to first-order theorem prover language.
- [bool2dimacs](https://github.com/Rose1917/bool2dimacs) [:package:](https://crates.io/crates/bool2cnf) - transfer boolean expression to dimacs directly.
- [CNFGEN](https://github.com/matszpk/cnfgen) [:package:](https://crates.io/crates/cnfgen) - create boolean formulae from boolean expressions and integer expressions.
- [Cnfpack](https://github.com/jix/cnfpack) [:package:](https://crates.io/crates/cnfpack) - converts between DIMACS CNF file format and the compressed binary Cnfpack format.
- [Decdnnf-rs](https://github.com/crillab/decdnnf_rs) [:package:](https://crates.io/crates/decdnnf_rs) - translating formulas generated by [d4](https://www.cril.univ-artois.fr/software/d4) into the format generated by [c2d](http://reasoning.cs.ucla.edu/c2d).
- [hz-to-mm0](https://github.com/digama0/hz-to-mm0) :zzz: - translator from HOL Zero / Common HOL to Metamath Zero.
- [Metamath hammer](https://github.com/digama0/mm-hammer) - tool for automatically proving Metamath theorems using ATPs.
- [rust-smt-ir](https://github.com/awslabs/rust-smt-ir) [:package:](https://crates.io/crates/aws-smt-ir)[:package:](https://crates.io/crates/aws-smt-ir-derive):star: - intermediate representation (IR) in Rust for SMT-LIB queries.

#### Misc

- [AbsoluteUnity](https://github.com/ray-kast/AbsoluteUnity) :zzz: - think Prolog, but less capable.
- [Alice_rs](https://github.com/firefighterduck/alice_rs) [:lab_coat:](http://www0.cs.ucl.ac.uk/staff/p.ohearn/papers/unroll_collapse_withproofs.pdf)[:lab_coat:](https://www21.in.tum.de/teaching/sar/SS20/8.pdf):zzz: - implementation of a decision procedure for A Decidable Fragment of Separation Logic.
- [auto](https://github.com/elliottt/auto) [:lab_coat:](https://www.jstor.org/stable/2275431) - decision procedure for intuitionistic logic.
- [Avatar Hypergraph Rewriting](https://github.com/advancedresearch/avatar_hypergraph_rewriting) [:package:](https://crates.io/crates/avatar_hypergraph_rewriting):zzz: - hypergraph rewriting system with avatars for symbolic distinction.
- [coc](https://github.com/azdavis/coc) :zzz: - the calculus of constructions.
- [compiler](https://github.com/trivial-rs/compiler) [:package:](https://crates.io/crates/trivial-compiler):baby_chick::zzz: - trivial compiler framework for Metamath Zero binary proofs.
- [discrimination-tree](https://github.com/MichaelRawson/discrimination-tree) [:package:](https://crates.io/crates/discrimination-tree) - discrimination tree term indexing.
- [easy-smt](https://github.com/elliottt/easy-smt) [:package:](https://crates.io/crates/easy-smt):star: - easy SMT solver interaction (Inspired by the [simple-smt haskell](https://hackage.haskell.org/package/simple-smt) package.).
- [egg](https://github.com/egraphs-good/egg) [:package:](https://crates.io/crates/egg):star: - flexible, high-performance e-graph library.
- [epilog](https://github.com/ray-kast/epilog) [:package:](https://crates.io/crates/epilog):zzz: - collection of Prolog-like tools for inference logic.
- [FALL](https://github.com/remexre/fall) [:package:](https://crates.io/crates/fall):zzz: - easily embeddable, futures-friendly logic engine.
- [foliage](https://github.com/potassco/foliage) [:package:](https://crates.io/crates/foliage):zzz: - first-order logic with integer arithmetics.
- [fuzzylogic](https://github.com/weirdsmiley/fuzzylogic) [:package:](https://crates.io/crates/fuzzylogic) - provides operations and inference for fuzzy set theory.
- [Joker Calculus](https://github.com/advancedresearch/joker_calculus.git) [:package:](https://crates.io/crates/joker_calculus) -  implementation of Joker Calculus in Rust.
- [Kravanenn](https://github.com/ppedrot/kravanenn) :star::zzz: - set of tools for Coq.
- [logic-lang](https://github.com/logic-lang/logic) [:package:](https://crates.io/crates/logic-lang) - structural logic based on equivalence graphs.
- [logical_solver](https://github.com/antoKeinanen/logical_solver-rs) [:package:](https://crates.io/crates/logical_solver):baby_chick: -  library for solving and parsing logical equations.
- [LogicNG](https://github.com/booleworks/logicng-rs) [:package:](https://crates.io/crates/logicng) - library for creating, manipulating and solving Boolean and Pseudo-Boolean formulas.
- [LogRu](https://github.com/fatho/logru) [:package:](https://crates.io/crates/logru) - small, embeddable and fast interpreter for a subset of Prolog.
- [mm0-rs](https://github.com/digama0/mm0/tree/master/mm0-rs) [:package:](https://crates.io/crates/mm0b_parser)[:package:](https://crates.io/crates/mm0_deepsize)[:package:](https://crates.io/crates/mm0_util):star:[:lab_coat:](https://digama0.github.io/mm0/thesis-slides.pdf)[:lab_coat:](https://digama0.github.io/mm0/thesis.pdf) - MM0/MM1 server and utilities.
- [mmb-binutils](https://github.com/trivial-rs/mmb-binutils) :zzz: - utility tools for Metamath Zero binary proof files.
- [mmb-types](https://github.com/trivial-rs/mmb-types) [:package:](https://crates.io/crates/mmb-types):zzz: - library containing the definitions of the opcodes in the Metamath Zero binary proof files.
- [moniker](https://github.com/brendanzab/moniker) [:package:](https://crates.io/crates/moniker)[:package:](https://crates.io/crates/moniker-derive):star::zzz: - automagical variable binding library.
- [nanoda](https://github.com/ammkrn/nanoda) :star::skull: - became nanoda-lib.
- [nanoda_lib](https://github.com/ammkrn/nanoda_lib) - type inference/checking functionality based on the Lean theorem prover.
- [nnf](https://github.com/night-crawler/nnf) [:package:](https://crates.io/crates/nnf) - Negation Normal Form manipulation library.
- [polytype](https://github.com/lucasem/polytype-rs) [:package:](https://crates.io/crates/polytype):star: - Hindley-Milner polymorphic typing system.
- [program-induction](https://github.com/lucasem/program-induction) [:package:](https://crates.io/crates/programinduction):star: - library for program induction and learning representations.
- [ruler](https://github.com/uwplse/ruler) :diamonds::star:[:lab_coat:](https://dl.acm.org/doi/10.1145/3485496) - rewrite rule inference using equality saturation.
- [Rust First Order Logic](https://github.com/BenRogersNewsome/First-Order-Logic) [:package:](https://crates.io/crates/first_order_logic) - syntax of First Order Logic with self-consistent logical assertions.
- [rust-nbe-for-mltt](https://github.com/brendanzab/rust-nbe-for-mltt) :star: - normalization by evaluation for Martin-Löf Type Theory with dependent records.
- [rust-smt-strings](https://github.com/awslabs/rust-smt-strings) [:package:](https://crates.io/crates/aws-smt-strings) - library for strings as defined in the SMT-LIB theory of strings.
- [~~rust-unify~~](https://github.com/bongo227/rust-unify) [:package:](https://crates.io/crates/rust-unify) :recycle: - unification algorithum implementation.
- [rustsat](https://github.com/chrjabs/rustsat) [:package:](https://crates.io/crates/rustsat)[:package:](https://crates.io/crates/rustsat-batsat)[:package:](https://crates.io/crates/rustsat-cadical)[:package:](https://crates.io/crates/rustsat-glucose)[:package:](https://crates.io/crates/rustsat-ipasir)[:package:](https://crates.io/crates/rustsat-kissat)[:package:](https://crates.io/crates/rustsat-minisat)[:package:](https://crates.io/crates/rustsat-tools) - provide elements commonly used in satisfiability solving software.
- [Rusty Razor](https://github.com/salmans/rusty-razor) [:package:](https://crates.io/crates/razor)[:package:](https://crates.io/crates/razor-fol)[:package:](https://crates.io/crates/razor-chase):star::zzz: - tool for constructing finite models for first-order theories.
- [sat_toasty_helper](https://github.com/Nathan-Fenner/sat_toasty_helper) [:package:](https://crates.io/crates/sat_toasty_helper) - convenient way to write and solve SAT constraints.
- [Satoxid](https://github.com/neuring/satoxid) [:package:](https://crates.io/crates/satoxid) - library to help with encoding SAT problems.
- [smt2utils](https://github.com/facebookincubator/smt2utils) [:package:](https://crates.io/crates/smt2parser)[:package:](https://crates.io/crates/smt2patch)[:package:](https://crates.io/crates/smt2proxy)[:package:](https://crates.io/crates/z3tracer):skull: - libraries and tools for the SMT-LIB-2 standard.
- [smtlib-syntax](https://github.com/keks/smtlib-rs) [:package:](https://crates.io/crates/smtlib-syntax) - syntactic types the  for the SMT-LIB 2.6 spec. Meant for code generation, not parsing.
- [term-rewriting-rs](https://github.com/joshrule/term-rewriting-rs) [:package:](https://crates.io/crates/term_rewriting):star::zzz: - representing, parsing, and computing with first-order term rewriting systems.
- [tribool](https://github.com/novacrazy/rust-tribool) [:package:](https://crates.io/crates/tribool):zzz: - three-valued logic.
- [The Trivial Metamath Zero kernel](https://github.com/trivial-rs/kernel) [:package:](https://crates.io/crates/trivial-kernel):zzz: - Metamath Zero kernel for Trivial.
- [Whisper](https://github.com/sdleffler/whisper) :star::zzz: - logic Programming DSL.

## Books code

*There is [numerous](https://github.com/search?l=Rust&q=tapl&type=Repositories) implementations of TAPL [:book:](https://www.cis.upenn.edu/~bcpierce/tapl), we keep only the most popular and keep an eye on implementations that worth attention.*

- [logic-rs](https://github.com/ixjf/logic-rs) [:book:](https://ruccs.rutgers.edu/lepore-meaning-and-argument/lepore-about-the-book):star::zzz: - parser of relational predicate logic & truth tree solver
- [plar-rs](https://github.com/nikomatsakis/plar-rs) [:book:](https://www.cl.cam.ac.uk/~jrh13/atp):zzz:[:ghost:](https://github.com/newca12/plar-rs) - exploring John Harrison's Handbook of Practical Logic and Automated Reasoning.
- [tapl](https://github.com/v4kst1z/tapl) :zzz: - implementation of TAPL.
- [TAPL in Rust](https://github.com/hayatoito/tapl-in-rust) :star::zzz: - another collection of implementations of TAPL.
- [The Little Prover](https://github.com/mbillingr/the-little-prover) [:book:](https://mitpress.mit.edu/9780262330572/the-little-prover) - transpiled J-Bob assistant & GUI frontend.
- [the-little-typer](https://github.com/mbillingr/the-little-typer) [:book:](https://mitpress.mit.edu/9780262536431/the-little-typer) - a Rust take on D.Friedman's book.
- [tnt](https://github.com/SymmetricChaos/tnt) [:book:](https://en.wikipedia.org/wiki/G%C3%B6del,_Escher,_Bach)[:package:](https://crates.io/crates/tnt) - implementation of Hofstader's "Typographical Number Theory" from the book Gödel, Escher & Bach.
- [types-and-programming-languages](https://github.com/lazear/types-and-programming-languages) :star::zzz: - Exercises from Benjamin Pierce's TAPL textbook + extras!

## Programming Language

- [beta](https://github.com/ReubenHillyard/beta) - dependently-typed programming language, aiming to support a cubical interpretation of univalence.
- [egglog](https://github.com/egraphs-good/egglog) [:package:](https://crates.io/crates/egglog):star:[:lab_coat:](https://arxiv.org/abs/2304.04332) - language that combines the benefits of equality saturation and datalog.
- [Fathom](https://github.com/yeslogic/fathom) [:package:](https://crates.io/crates/fathom):star::construction: - declarative data definition language for formally specifying binary data formats.
- [High-order Virtual Machine (HVM)](https://github.com/HigherOrderCO/HVM) :star: - massively parallel, optimal functional runtime.
- [isotope-prover-experiments](https://gitlab.com/tekne/isotope-prover-experiments) [:lab_coat:](https://gitlab.com/tekne/phd-proposal/-/blob/main/report.tex)[:lab_coat:](https://gitlab.com/isotope-project/msc-thesis/-/blob/master/thesis.tex):skull: - experimental dependently typed language supporting borrow checking.
- [Kind](https://github.com/HigherOrderCO/Kind) [:package:](https://crates.io/crates/kind2):star: - next-gen functional language and proof assistant.
- [Last Order Logic](https://github.com/advancedresearch/last_order_logic.git) [:package:](https://crates.io/crates/last_order_logic) - experimental logical language.
- [minihl](https://github.com/firefighterduck/minihl) - formal methods playgorund for MiniHeapLang language.
- [minitt-rs](https://github.com/owo-lang/minitt-rs) [:package:](https://crates.io/crates/minitt)[:package:](https://crates.io/crates/minitt-util):star::skull: - became Voile.
- [Narc](https://github.com/owo-lang/narc-rs) [:package:](https://crates.io/crates/nar):star::zzz: - dependently-typed programming language with Agda style dependent pattern matching.
- [Pika](https://github.com/tolziplohu/pika) :star::construction: - small, performance-oriented, dependently typed ML with algebraic effects and unboxed types..
- [Pikelet](https://github.com/pikelet-lang/pikelet) [:package:](https://crates.io/crates/pikelet):star::zzz: - small, functional, dependently typed programming language.
- [proto-vulcan](https://github.com/terohuttunen/proto-vulcan) [:package:](https://crates.io/crates/proto-vulcan)[:package:](https://crates.io/crates/proto-vulcan-macros) - miniKanren-family relational logic programming language.
- [rooc](https://github.com/Specy/rooc) :mortar_board::star: - a language for compiling formal mathematical models into static models.
- [Rust pi-forall](https://github.com/sourcedennis/rust-pi-forall) [:lab_coat:](https://github.com/sweirich/pi-forall/blob/2022/doc/oplss.pdf) - partial re-implementation of pi-forall.
- [Scryer Prolog](https://github.com/mthom/scryer-prolog) [:package:](https://crates.io/crates/scryer-prolog):star: - modern Prolog implementation.
- [SMT-language](https://github.com/DavidD12/smt-lang) [:package:](https://crates.io/crates/smt-lang) - Sat Modulo Theory Language.
- [stupid-see](https://github.com/Hoblovski/stupid-see) :baby_chick::zzz: - symbolic execution engine. Mainly targeted at the verification course in THU.
- [Symmetric Interaction Calculus](https://github.com/maiavictor/symmetric-interaction-calculus) :star::skull: - optimal λ-calculus reduction. Followed devlopment now in Kind project.
- [tako](https://github.com/Cypher1/tako) -  experimental programming language for ergonomic software verification.
- [TIP](https://github.com/v4kst1z/TIP) :baby_chick::zzz: - imperative programming language aimed at teaching fundamental concepts of static program analysis.
- [Untyped Concatenative Calculus](https://github.com/dawn-lang/ucc) :zzz: - toy programming language and prototype for [Dawn](https://www.dawn-lang.org).
- [Untyped Multistack Concatenative Calculus](https://github.com/dawn-lang/umcc) - toy programming language and prototype for [Dawn](https://www.dawn-lang.org).
- [Voile](https://github.com/owo-lang/voile-rs) [:package:](https://crates.io/crates/voile)[:package:](https://crates.io/crates/voile-util):star::zzz: - became Narc.
- [zz](https://github.com/zetzit/zz) [:package:](https://crates.io/crates/zz):star::skull: - zymbolic verifier and tranzpiler to bare metal C.

## Kanren

- [Canrun](https://github.com/tgecho/canrun_rs) [:package:](https://crates.io/crates/canrun):star: - logic programming library inspired by the *Kanren family of language DSLs.
- [miniKANREN](https://github.com/mbillingr/miniKANREN) [:package:](https://crates.io/crates/mini-kanren):zzz: - miniKANREN as a DSL.
- [rslogic](https://github.com/kulibali/rslogic) [:package:](https://crates.io/crates/rslogic):star::zzz: - logic programming framework for Rust inspired by µKanren.
- [rust-kanren](https://github.com/wartmanm/rust-kanren) :star::zzz: - loose interpretation of miniKanren and cKanren.
- [µKanren-rs](https://github.com/ekzhang/ukanren-rs) [:package:](https://crates.io/crates/ukanren):star: - implementation of µKanren.

## Lambda Calculus

- [blc](https://github.com/ljedrz/blc) [:package:](https://crates.io/crates/blc):zzz: - implementation of the binary lambda calculus.
- [Closure Calculus](https://github.com/advancedresearch/closure_calculus) [:package:](https://crates.io/crates/closure_calculus)[:lab_coat:](https://dl.acm.org/doi/abs/10.1145/3294032.3294085):zzz: - library for Barry Jay's Closure Calculus.
- [lam](https://github.com/pro465/lam) - lambda calculus evaluator.
- [Lamb](https://github.com/Carnagion/lamb) [:package:](https://crates.io/crates/lamb):mortar_board: - implementation of the pure untyped lambda calculus in modern, safe Rust.
- [lambash](https://github.com/nixpulvis/lambash) [:package:](https://crates.io/crates/lambash):zzz: - λ-calculus shell.
- [~~lambda_calc~~](https://gitlab.com/mcmfb/lambda-calculator) [:package:](https://crates.io/crates/lambda_calc):recycle: - command-line untyped lambda calculus interpreter.
- [lambda_calculus](https://github.com/ljedrz/lambda_calculus) [:package:](https://crates.io/crates/lambda_calculus):star: - simple, zero-dependency implementation of pure lambda calculus in safe Rust.
- [lambda_calculus](https://github.com/thomasdziedzic/lambda_calculus) :zzz: - lambda calculus with antlr grammar.
- [lambdacube](https://github.com/felixzhuologist/lambdacube) :construction::zzz: - implementation of the lambda cube (and other type stuff).
- [Lambda Shell](https://github.com/jzbor/lash) [:package:](https://crates.io/crates/lash) - simple REPL shell for untyped lambda expressions.
- [Lambdascript](https://github.com/chuckcscccl/lambdascript) - educational tool illustrating beta reduction of untyped lamba terms.
- [Lamcal](https://github.com/haraldmaida/lamcal) [:package:](https://crates.io/crates/lamcal)[:package:](https://crates.io/crates/lamcal-repl):zzz: - lambda calculus parser and evaluator and a separate command line REPL.
- [lalrpop-lambda](https://github.com/nixpulvis/lalrpop-lambda) [:package:](https://crates.io/crates/lalrpop-lambda):star: - λ-calculus grammar/interpretor written using LALRPOP and `λ!`.
- [Pun Calculus](https://github.com/andrew-johnson-4/PunCalculus) [:package:](https://crates.io/crates/punc) - variant of Typed Lambda Calculus with generalized variable punning (ad-hoc polymorphism).
- [RLCI](https://github.com/orsinium-labs/rlci) :star: - Overly-documented Lambda Calculus Interpreter.
- [type-theory](https://github.com/segeljakt/type-theory) :star: - typed λ-calculus.

## Propositional logic

- [~~Chevre~~](https://github.com/pvdrz/chevre) :recycle: - small propositional logic interpreter.
- [implies](https://github.com/armaan-rashid/implies) [:package:](https://crates.io/crates/implies) - storing logical formulas as parse trees and performing complex operations on them.
- [logic](https://github.com/nextzhou/logic) [:package:](https://crates.io/crates/logic):baby_chick::zzz: - crate for propositional logic.
- [logic-resolver](https://github.com/gustafla/logic-resolver) :baby_chick::zzz: - toy implementation of resolution for propositional logic.
- [mini-prop](https://github.com/emilHof/mini-prop) [:package:](https://crates.io/crates/mini-prop) - CLI tool for parsing and processing LaTex formatted propositional statements.
- [plc](https://github.com/trolleyman/plc) :zzz: - propositional logic calculator.
- [Plogic](https://github.com/Janko-dev/plogic) :star: - propositional logic evaluator and rule-based pattern matcher.
- [Prop](https://github.com/advancedresearch/prop) [:package:](https://crates.io/crates/prop):star: - library for theorem proving with Intuitionistic Propositional Logic.
- [Propositional Logic](https://github.com/PawelJastrzebski/propositional) [:package:](https://crates.io/crates/propositional):mortar_board: - propositional Logic Library .
- [Propositional Tableaux Solver](https://github.com/jieyouxu/propositional-tableau-solver-rs) [:package:](https://crates.io/crates/propositional-tableau-solver-rs):zzz: - solver using the propositional tableaux method.
- [prop_tune](https://github.com/emilHof/prop_tune) [:package:](https://crates.io/crates/prop_tune)[:package:](https://crates.io/crates/prop_tune_core)[:package:](https://crates.io/crates/prop_tune_macro) - library for working with Logical Propositions.
- [raa_tt](https://github.com/jsinger67/raa_tt) [:package:](https://crates.io/crates/raa_tt) - prover for sentences of propositional calculus.
- [Resolution Prover](https://github.com/ExcaliburZero/resolution-prover) :zzz: - resolution prover library for propositional logic.
- [resolution-prover](https://github.com/arbaregni/resolution-prover) :zzz: - Uses propositional resolution to prove statements and proofs on discord.
- [rs-logik](https://github.com/SolarLiner/rs-logik) [:ghost:](https://github.com/newca12/rs-logik) - propositional logic interpreter.
- [rust-proplogic-toylang](https://github.com/SnO2WMaN/rust-proplogic-toylang) :baby_chick: - toy language for Propositional Logic.
- [rusty-logic](https://github.com/mcheatham/rusty-logic) :baby_chick::zzz: - propositional logic analysis.
- [simple-proof-assistant](https://github.com/long-long-float/simple-proof-assistant) :baby_chick::zzz: - a proof assistant kernel for minimal propositional logic.
- [validator](https://github.com/Maaarcocr/validator) :zzz: - small utility to test a propositional logic theorem prover.

## Unclassified

- [Croissant](https://github.com/super7ramp/croissant) - crossword solver backed by various SAT solvers.
- [formal-systems-learning-rs](https://github.com/joshrule/formal-systems-learning-rs) :zzz: - simulations to learn formal systems as typed first-order term rewriting systems.
- [Hashi - Bridges Puzzle](https://github.com/NoelHuibers/Hashiwokakero) - Hashi Puzzle (aka Bridges) solver.
- [inf402](https://github.com/edgarogh/inf402) - SAT-solver-based takuzu solver.
- [Junglefowl](https://github.com/wrsturgeon/junglefowl) [:package:](https://crates.io/crates/junglefowl)[:package:](https://crates.io/crates/junglefowl-macros) - runs Peano arithmetic on Rust types, verified at compile time..
- [list-routine-learning-rs](https://github.com/joshrule/list-routine-learning-rs) :zzz: - to learn typed first-order term rewriting systems that perform list routines.
- [logical_tui](https://github.com/antoKeinanen/logical_tui) :baby_chick: - tui for  [logical_solver](https://github.com/antoKeinanen/logical_solver-rs).
- [Minimal models](https://github.com/jix/minimal_models_example) :zzz: - uses a SAT solver to find minimal partial assignments that are model of a CNF formula.
- [n-queens-sat](https://github.com/erohkohl/n-queens-sat) :zzz: - modelling n-queens problem as conjunctive normal form and solving it with DPLL algorithm.
- [nonogrid](https://github.com/tsionyx/nonogrid) [:package:](https://crates.io/crates/nonogrid) - lightning fast nonogram solver.
- [Relog](https://github.com/andrew-johnson-4/InPlace) - implementation of several strongly-normalizing string rewriting systems.
- [roq](https://github.com/wgoodall01/roq) [:package:](https://crates.io/crates/roq)[:package:](https://crates.io/crates/roq_derive) - proc-macro Coq code generation and proof automation.
- [rummy_to_sat ](https://github.com/neuring/rummy_to_sat) - implementation of a solver for [Rummy](https://en.wikipedia.org/wiki/Rummy).
- [rust-z3-practice](https://github.com/salmans/rust-z3-practice) :zzz: - solving a number of SAT problems using Z3.
- [sudoku_sat](https://github.com/shnarazk/sudoku_sat) - solve Sudoku variants with SAT solvers.
- [Supermux](https://github.com/tuzz/supermux) :zzz: - reduction of the superpermutation problem to Quantified Boolean Formula.
- [Supersat](https://github.com/tuzz/supersat) :zzz: - attempt to find superpermutations by reducing the problem to SAT.
- [tarpit-rs](https://github.com/sdleffler/tarpit-rs) :star::zzz: - type-level implementation of Smallfuck. Turing-completeness proof for Rust's type system.
- [VeriFactory](https://github.com/alegnani/verifactory) :star: - verifier for [Factorio blueprints](https://factorioprints.com).

## Resources

### Books

- [Verification for Dummies: SMT and Induction](https://ocamlpro.github.io/verification_for_dummies) - broadly discusses induction as a formal verification technique.

### Research Paper & Thesis

- [How to discover short, shorter, and the shortest proofs of unsatisfiability](https://arxiv.org/pdf/2411.07955)[:factory:](https://zenodo.org/records/14051922) - 2024
- [A hybrid approach to semi-automated Rust verification](https://arxiv.org/pdf/2403.15122) - 2024.
- [Verification of a Rust Implementation of Knuth's Dancing Links using ACL2](https://arxiv.org/abs/2311.08862v1) - 2023.
- [Specifying and Verifying Higher-order Rust Iterators](https://hal.science/hal-03827702v2/document) - 2023.
- [RustHornBelt: A Semantic Foundation for Functional Verification of Rust Programs with Unsafe Code](https://www.lri.fr/~xldenis/paper/rusthornbelt.pdf) - 2022.
- [Hardware/Software Co-Assurance using the Rust Programming Language and ACL2](https://arxiv.org/abs/2205.11709v1) - 2022.
- [Extensible Functional-Correctness Verification of Rust Programs by the Technique of Prophecy](https://github.com/shiatsumat/master-thesis) - 2021.
- [Understanding and Evolving the Rust Programming Language](https://www.ralfj.de/research/thesis.html) - 2020.
- [Simple Verification of Rust Programs via Functional Purification](https://pp.ipd.kit.edu/uploads/publikationen/ullrich16masterarbeit.pdf) - 2016.

### Demos

- [Artifact Evaluation: Kani Rust Verifier](https://github.com/avanhatt/icse22ae-kani) [:lab_coat:](https://www.cs.cornell.edu/~avh/dyn-trait-icse-seip-2022-preprint.pdf) - Kani Rust Model Checker artifact for ICSE 2022 Artifact Evaluation.
- [flux-demo](https://github.com/flux-rs/flux-demo) - small examples that demonstrate how flux works.
- [rust-smt-ir-examples](https://github.com/awslabs/rust-smt-ir-examples) - examples of using a rust-smt-ir, a Rust intermediate representation (IR) for SMT-LIB.
- [aws-lambda-z3](https://github.com/sourcedennis/aws-lambda-z3) - tutorial on running Z3 on AWS Lambda, with Rust.

### Blogs

- [A Formal Verification of Rust's Binary Search Implementation.](https://kha.github.io) :uk:
- [Formal Land](https://formal.land/blog) :uk:
- [Kani Rust Verifier Blog](https://model-checking.github.io/kani-verifier-blog) :uk:
- [Mist Blog](https://mist.bvng.dk) :uk:
- [Splr notebook.](https://shnarazk.github.io/tags/#splr) :jp:
- [Research notebook about improving with Rust the performance of nonclausal automated theorem provers.](https://github.com/01mf02/adam-notes) :uk::diamonds:
- [Articles about a collection of tools/libraries to support both static and dynamic verification of Rust programs.](https://project-oak.github.io/rust-verification-tools) :uk:
- [Varisat notebook.](https://jix.one/blog/sat) :uk::diamonds:

### Posts

- [Visions of the future: formal verification in Rust](https://xav.io/blog/rust-formal-verification) - 2024
- [Some notes on Rust, mutable aliasing and formal verification](https://graydon2.dreamwidth.org/312681.html) :diamonds: - 2024
- [Cracking the Cryptic (with Z3 and Rust)](https://hugopeters.me/posts/21) - 2024
- [How Open Source Projects are Using Kani to Write Better Software in Rust](https://aws.amazon.com/fr/blogs/opensource/how-open-source-projects-are-using-kani-to-write-better-software-in-rust) - 2023.
- [Check AI-Generated Code Perfectly and Automatically](https://medium.com/@carlmkadie/check-ai-generated-code-perfectly-and-automatically-d5b61acff741) - 2023.
- [Solving The Witness with Z3](https://www.techofnote.com/witness-part-1) - 2022.
- [Formally Verifying Rust's Opaque Types](https://dylanj.xyz/posts/rust-coq-opaque-types) - 2022.
- [An adventure with optimization, Rust and Z3](https://ochagavia.nl/blog/an-adventure-with-optimization-rust-and-z3) - 2019.

### Crates keywords

- [solver](https://crates.io/keywords/solver) - 126 entries. :100:
- [logic](https://crates.io/keywords/logic) - 87 entries. :100:
- [verification](https://crates.io/keywords/verification) - 48 entries. :100:
- [smt](https://crates.io/keywords/smt) - 43 entries. :100:
- [sat](https://crates.io/keywords/sat) - 38 entries. :100:
- [satisfiability](https://crates.io/keywords/satisfiability) - 26 entries. :100:
- [linear-programming](https://crates.io/keywords/linear-programming) - 17 entries. :100:
- [proving](https://crates.io/keywords/proving) - 13 entries. :100:
- [smt-lib](https://crates.io/keywords/smt-lib) - 12 entries. :100:
- [cnf](https://crates.io/keywords/cnf) - 10 entries. :100:
- [rewriting](https://crates.io/keywords/rewriting) - 9 entries. :100:
- [prover](https://crates.io/keywords/prover) - 8 entries. :100:
- [sat-solver](https://crates.io/keywords/sat-solver) - 8 entries. :100:
- [first-order](https://crates.io/keywords/first-order) - 6 entries. :100:
- [z3](https://crates.io/keywords/z3) - 6 entries. :100:
- [dependent-types](https://crates.io/keywords/dependent-types) - 6 entries. :100:
- [metamath-zero](https://crates.io/keywords/metamath-zero) - 5 entries. :100:
- [dimacs](https://crates.io/keywords/dimacs) - 5 entries. :100:

### Community

- [Mikko Aarnos](https://github.com/mAarnos) - Serkr.
- [Johannes Altmanninger](https://github.com/krobelus) - rate.
- [ammkrn](https://twitter.com/ammkrn) - nanoda, nanoda_lib, second_opinion.
- [Bruno Andreotti](https://github.com/bpandreotti) - Carcara.
- [Arata](https://github.com/arata-nvm) - lutrix.
- [arbaregni](https://github.com/arbaregni) - resolution-prover.
- [astrobeastie](https://github.com/astrobeastie) - sequentprover.
- [Yechan Bae](https://qwaz.github.io) - Rudra, Satire.
- [Clark Barrett](https://github.com/cbarrettfb) - Rust-SMT-LIB-API.
- [Mathieu Baudet](https://github.com/ma2bd) - smt2utils.
- [Mike Beaumont](https://github.com/michaelbeaumont) - rust-sat.
- [Antoine Belvire](https://github.com/super7ramp) - Croissant.
- [Tim Beurskens](https://timbeurskens.github.io) - RsBDD.
- [Matteo Biggio](https://github.com/mbiggio) - cplex-rs.
- [Justin Blanchard](https://github.com/UncombedCoconut) - cat_solver.
- [boitsov14](https://github.com/boitsov14) - theorem-prover-rs.
- [James Bornholt](https://www.cs.utexas.edu/~bornholt) - rustsat(2), Shuttle.
- [Henrik Böving](https://github.com/hargoniX) - Obvious.
- [Oliver Bøving](https://github.com/oeb25) - Mist, smtlib, vipers.
- [Lee ByeongJun](https://github.com/notJoon) - Lambda Calculus Parser.
- [Bickio O'Callahan](https://github.com/Bickio) - Solving The Witness with Z3.
- [Mario Carneiro](https://github.com/digama0) - coq-rs, FRAT-rs, hz-to-mm0, isabelle export tool, Metamath hammer, Metamath-knife, Mizar proof checker, mm0-rs, olean-rs.
- [Tej Chajed](https://github.com/tchajed) - Temporal Verifier.
- [Adrien Champion](https://github.com/AdrienChampion) - hoice, Kinō, matla, Mikino, rsmt2, SAT-MICRO, Verification for Dummies.
- [David Chanin](https://github.com/chanind) - Tensor Theorem Prover.
- [Michelle Cheatham](https://github.com/mcheatham) -  rusty-logic.
- [Jimmy Chen Chen](https://github.com/jchenche) - theorem-prover.
- [Alex Chew](https://github.com/alex-chew) - Z3D.
- [Konstantin Chukharev](https://github.com/Lipen) - SAT Nexus, backdoor-solver.
- [Guillaume Claret](https://github.com/clarus) - coq-of-rust, Formal Land.
- [Cobalt](https://cobalt.rocks/) - SAT solver ANalyser.
- [Lorenzo Colombini](https://github.com/Lorenzinco) - Colombini-SAT.
- [convexbrain](https://github.com/convexbrain) - Totsu.
- [David Cox](https://github.com/david-r-cox) - mps.
- [Simon Cruanes](https://simon.cedeela.fr) - BatSat.
- [Dacit](https://github.com/Dacit) - Sequent solver.
- [dandxy89](https://github.com/dandxy89) - lp_parser_rs.
- [Azeez Daoud](https://azeezda.github.io/portfolio) - ceetle.
- [DavidD12](https://github.com/DavidD12) - SMT-language, smt_sb-rs.
- [Ariel Davis](https://azdavis.net) - coc.
- [Xavier Denis](https://www.lri.fr/membre_en.php?mb=2819) - Creusot, RustHornBelt: A Semantic Foundation for Functional Verification of Rust Programs with Unsafe Code, RustHornBelt Library & Benchmarks, Rust verification tools (2021), Specifying and Verifying Higher-order Rust Iterators (2023), A hybrid approach to semi-automated Rust verification (2024), Visions of the future: formal verification in Rust.
- [Sushant Dinesh](https://github.com/sushant94) - libsmt.rs.
- [Sylvie Dirkswager](https://github.com/tolziplohu) - Pika.
- [Craig Disselkoen](https://cseweb.ucsd.edu/~cdisselk) - boolector.
- [Mark Drobnak](https://github.com/AzureMarker) - p4-analyzer.
- [Bruno Dutertre](https://github.com/BrunoDutertre) - rust-smt-ir, rust-smt-ir-examples, rust-smt-strings.
- [Thomas Dziedzic](https://www.thomasdziedzic0.com) - lambda_calculus.
- [Kurt Ehlert](https://github.com/kehlert) - ellp.
- [Trevor Elliott](https://github.com/elliottt) - auto, easy-smt.
- [endeav0r](https://github.com/endeav0r) - falcon-z3.
- [Enkelmann](https://github.com/Enkelmann) - cwe_checker.
- [Aodhnait Étaín](https://aodhneine.github.io) - Esther.
- [Michael Färber](http://cl-informatik.uibk.ac.at/users/mfaerber) - CoP, Kontroli, Lambda Term Parsing, meancop, research notebook about improving with Rust the performance of nonclausal automated theorem provers.
- [Nathan Fenner](https://github.com/Nathan-Fenner) - sat_toasty_helper.
- [FireFighterDuck](https://github.com/firefighterduck) - Alice_rs, Kissat-rs, minihl.
- [Paolo Flores](https://www.paoloose.site) - logic-parser.
- [Hugo Frezat](https://github.com/hrkz) - logic-lang.
- [Robin Freyler](https://robbepop.github.io) - CNF Parser, DIMACS Parser, Stevia.
- [Lennard Gäher](https://gitlab.mpi-sws.org/lgaeher) - RefinedRust.
- [Galois, Inc.](http://galois.com) - crux-mir.
- [Alexey Gerasimov](https://github.com/fan-tom) - Liquid Rust.
- [Jad Ghalayini](https://gitlab.com/tekne) - isotope-prover-experiments, lean-sys.
- [Mohammed Ghannam](https://github.com/mmghannam) - russcip, scip-sys.
- [Nathan Graule ](https://github.com/SolarLiner) - rs-logik.
- [Brandon H. Gomes](https://github.com/bhgomes) - qbar.
- [William Goodall](https://github.com/wgoodall01) - roq.
- [Robert Grosse](https://github.com/Storyyeller) - cryptominisat-rs.
- [Masaki Hara](https://twitter.com/qnighy) - Logic solver, RatSat.
- [Jannis Harder](https://jix.one) - Cnfpack, Flussab CNF, Minimal models, starlit, Varisat, Varisat notebook.
- [David S. Hardin](https://github.com/david-s-hardin) - Hardware/Software Co-Assurance using the Rust Programming Language and ACL2, Verification of a Rust Implementation of Knuth's Dancing Links using ACL2.
- [Rowan Hart](https://github.com/novafacing) - Yices2.
- [Timothée Haudebourg](https://github.com/timothee-haudebourg) - smt2.
- [Reuben Hillyard](https://github.com/ReubenHillyard) - beta.
- [Son HO](https://github.com/sonmarcho) - Charon.
- [Sarek Høverstad Skotåm](https://github.com/sarsko) - CreuSAT.
- [Hoblovski](https://github.com/Hoblovski) - stupid-see, stupid-smt.
- [Graydon Hoare](https://github.com/graydon) - Some notes on Rust, mutable aliasing and formal verification.
- [Emil Hofstetter](https://emilhofstetter.dev) - mini-prop, prop_tune.
- [hrkzmnm](https://github.com/hrkzmnm) - rust_z3prover.
- [Tero Huttunen](https://github.com/terohuttunen) - proto-vulcan.
- [Noel Huibers](https://github.com/NoelHuibers) - Hashi - Bridges Puzzle.
- [Christoph Jabs](https://github.com/chrjabs) - Scuttle, maxpre-rs, rustsat.
- [Jan](https://github.com/Janko-dev) - Plogic.
- [Paweł Jastrzebski](https://github.com/PawelJastrzebski) - Propositional Logic.
- [Ranjit Jhala](https://github.com/ranjitjhala) - flux-demo.
- [Andrew Johnson](https://github.com/andrew-johnson-4) - LSTS, Pun Calculus, Relog.
- [Evan Johnson](https://github.com/enjhnsn2) - VeriWasm.
- [Dylan R. Johnston](https://dylanj.xyz) - Formally Verifying Rust's Opaque Types.
- [Matthias Jugan](https://github.com/Apfelbeet) - LogicNG, logicng-open-wbo-sys.
- [Ralf Jung](https://www.ralfj.de) - Understanding and Evolving the Rust Programming Language.
- [jzbor](https://github.com/jzbor) - Lambda Shell.
- [Carl Kadie](https://github.com/CarlKCarlK) - Check AI-Generated Code Perfectly and Automatically.
- [Hosein Kalbasi](https://github.com/HKalbasi) - akim.
- [Igor Kalichevski](https://github.com/night-crawler) - nnf.
- [karroffel](https://gitlab.com/karroffel) - contracts.
- [Anto Keinänen](https://github.com/antoKeinanen) - logical_solver, logical_tui.
- [Rahul Kumar](https://github.com/rahulku) - How Open Source Projects are Using Kani to Write Better Software in Rust.
- [Prateek Kumar](https://prateekkumar.in) - msat, rsat, slp, SolHOP.
- [Alexey Kutepov](https://tsoding.org) - Noq.
- [Ivan Ladelshchikov](https://github.com/tsionyx) - nonogrid.
- [Kevin Laeufer](https://github.com/ekiwi) - Patronus.
- [Aleksandr Larionov](https://github.com/snigavik) - bootfrost.
- [Andrea Lattuada](https://github.com/utaal) - verus.
- [lcnr](https://lcnr.de) - cobalt.
- [Shea Leffler](http://loud.fyi) - tarpit-rs, whisper.
- [Alessandro Legnani](https://github.com/alegnani) - VeriFactory.
- [Nico Lehmann](https://github.com/nilehmann) - Flux.
- [Carl Lerche](https://github.com/carllerche) - Loom.
- [Chuck Liang](https://github.com/chuckcscccl) - Lambdascript.
- [Nathan Lilienthal](https://nixpulvis.com/) - lambash, lalrpop-lambda.
- [ljedrz](https://github.com/ljedrz) - blc, lambda_calculus.
- [Ophir LOJKINE](https://github.com/lovasoa) - highs, highs-sys, good_lp.
- [Emmanuel Lonca](https://github.com/elonca) - Decdnnf-rs, Ipasir-loading, pblib-rs.
- [Kevin Lotz](https://github.com/lotzk) - isabelle-client.
- [Patrick Lühne](https://www.luehne.de) - anthem, foliage.
- [Michael Madden](https://github.com/mikemadden42) - Xori.
- [Scott J Maddox](https://github.com/scottjmaddox) - Untyped Concatenative Calculus, Untyped Multistack Concatenative Calculus.
- [Indraneel Mahendrakumar](https://github.com/Carnagion) - Lamb.
- [Harald Maida](https://github.com/haraldmaida) - Lamcal.
- [Krzysztof Małysa](https://github.com/varqox) - prover.
- [Manas](https://github.com/weirdsmiley) - fuzzylogic.
- [Miklos Maroti](https://www.math.u-szeged.hu/~mmaroti) - cadical-rs, relsat-rs, uasat-rs.
- [marshtompsxd](https://github.com/marshtompsxd) - verifiable-controllers.
- [Niko Matsakis](http://smallcultfollowing.com/babysteps) - Chalk, Kani, plar-rs.
- [Yusuke Matsushita](https://github.com/shiatsumat) - Extensible Functional-Correctness Verification of Rust Programs by the Technique of Prophecy, RustHorn.
- [mbillingr](https://github.com/mbillingr) - miniKANREN, The Little Prover, the-little-typer.
- [mcmfb](https://github.com/mcmfb) - lambda_calc.
- [Tom Meyer](https://github.com/Skasselbard) - Granite.
- [Alexander Mishunin](https://github.com/mishun) - minisat-rust.
- [Proloy Mishra](https://github.com/pro465) - lam, nnoq, nyaya.
- [Bruce Mitchener](https://github.com/waywardmonkeys) - z3.
- [Lucas Morales](https://lucasem.com) - polytype, program-induction.
- [Jesse Mu](https://github.com/jayelm) - satyrs.
- [Dominic Mulligan](https://dominicpm.github.io) - Supervisionary.
- [Jon Nadal](https://github.com/jonnadal) - Stateright.
- [Chandrakana Nandi](https://github.com/chandrakananandi) - Ruler.
- [neuring](https://github.com/neuring) - rummy_to_sat, Satoxid.
- [Sven Nilsen](https://github.com/bvssvni) - Avalog, Avatar Hypergraph Rewriting, Caso, Debug-SAT, Joker Calculus, Last Order Logic, linear_solver, Monotonic-Solver, pocket_prover, pocket_prover-set, Poi, Prop, reachability_solver.
- [Sven Thiele](https://github.com/sthiele) - clingo-rs.
- [Yuichi Nishiwaki](https://github.com/nyuichi) - shari.
- [Stefan O'Rear](https://github.com/sorear) - smetamath.
- [Robert Obkircher](https://github.com/RobertObkircher) - sat-solver.
- [Adolfo Ochagavía](https://ochagavia.nl) - An adventure with optimization, Rust and Z3.
- [Edgar Onghena](https://edgar.bzh/) - inf402.
- [Alex Ozdemir](https://cs.stanford.edu/~aozdemir) - rlfsc.
- [Chris Patuzzo](https://tuzz.tech) - Supermux, Supersat.
- [Pierre-Marie Pédrot](https://www.pédrot.fr) - Kravanenn.
- [Hugo Peters](https://github.com/HugoPeters1024) - Cracking the Cryptic (with Z3 and Rust).
- [Arvid E. Picciani](https://github.com/aep) - zz.
- [Dan Pittman](https://dpitt.me) - Bounded Registers.
- [Gabriel Poesia](https://github.com/gpoesia) - minimo.
- [Nadia Polikarpova](https://cseweb.ucsd.edu/~npolikarpova) - cyclegg.
- [Christian Poveda](https://github.com/pvdrz) - Chevre.
- [Bobby Powers](https://github.com/bpowers) - Logically Qualified Data Types.
- [Joshua Pratt](https://blog.mimir.systems) - ArcsJs - Provable, tako.
- [petersn](https://github.com/petersn) - autosat.
- [Boqin Qin](https://github.com/BurtonQin) - lockbud.
- [Armaan Rashid](https://github.com/armaan-rashid) - implies.
- [Michael Rawson](http://rawsons.uk/michael) - discrimination-tree, lazyCoP, lerna, lickety, SATCoP, tptp.
- [Alastair Reid](https://alastairreid.github.io) - Articles about a collection of tools/libraries to support both static and dynamic verification of Rust programs, Rust Software Verification Benchmarks, Rust verification tools, Rust verification tools list.
- [Adrien Renaudineau](https://github.com/arenaudineau) - sat_lab.
- [Corey Richardson](https://github.com/emberian) - lpsolve.
- [Nathan Ringo](https://remexre.xyz) - FALL.
- [Benjamin Rogers-Newsome](https://github.com/BenRogersNewsome) - Rust First Order Logic.
- [Erik Rohkohl](https://blogs.itemis.com/author/erik-rohkohl) - n-queens-sat.
- [Marco Concetto Rudilosso](https://github.com/Maaarcocr) - validator.
- [Josh Rule](http://www.joshrule.com) - formal-systems-learning-rs, list-routine-learning-rs, term-rewriting-rs. 
- [Salman Saghafi](https://github.com/salmans) - rust-z3-practice, Rusty Razor.
- [Michael Salter](https://github.com/salterm) - Rustproof, rustproof-libsmt.
- [Robert Scheidegger](https://github.com/RobScheidegger) - microsat.
- [Daniel Schemmel](https://daniel.schemmel.net) - DRSAT.
- [Ryan Schroeder](https://ryan-s.net) - AbsoluteUnity, epilog.
- [Carol Schulze](https://github.com/Ereski) - gpp-solver.
- [Klas Segeljakt](https://github.com/segeljakt) - type-theory.
- [shinkwhek](https://github.com/shinkwhek) - SAT solver.
- [skbaek](https://github.com/skbaek) - t3p.
- [Narazaki Shuji](https://shnarazk.github.io) - SAT-bench, Splr, Splr notebook, sudoku_sat.
- [Konstantin Sidorov](https://github.com/sidorov-ks) - How to discover short, shorter, and the shortest proofs of unsatisfiability, simple-stat.
- [Jörg Singer](https://github.com/jsinger67) - raa_tt.
- [J David Smith](https://github.com/emallson) - rplex.
- [SnO₂WMaN](https://github.com/SnO2WMaN) - rust-proplogic-toylang.
- [snsinfu](https://github.com/snsinfu) - dpll-sat.
- [Mikhail Solovev](https://github.com/fatemender) - bitwuzla-sys, boolector-sys.
- [Specy](https://github.com/Specy) - microlp, rooc.
- [Dennis Sprokholt](https://dennis.life) - aws-lambda-z3, Rust pi-forall.
- [Will Sturgeon](https://github.com/wrsturgeon) - Junglefowl.
- [Yuheng Su](https://github.com/gipsyh) - logic-form.
- [SymmetricChaos](https://github.com/SymmetricChaos) - tnt.
- [Mateusz Szpakowski](https://github.com/matszpk) - CNFGEN, Exec-SAT.
- [Lucas Tabary-Maujean](https://github.com/loutr) - Proost.
- [Victor Taelin](https://medium.com/@maiavictor) - High-order Virtual Machine (HVM), Kind2, Symmetric Interaction Calculus..
- [Calin Tataru](https://github.com/calintat) - homotopy-rs.
- [Mark Thom](https://github.com/mthom) - Scryer Prolog.
- [Fabian Thorand](https://github.com/fatho) - LogRu.
- [Hitoshi Togasaki](https://github.com/togatoga) - scrapsat, screwsat.
- [Callum Tolley](https://github.com/trolleyman) - plc
- [Aaron Trent](https://github.com/novacrazy) - tribool.
- [Sebastian Ullrich](https://twitter.com/derKha) - A Formal Verification of Rust's Binary Search Implementation, electrolysis, Simple Verification of Rust Programs via Functional Purification.
- [V4kst1z](https://github.com/v4kst1z) - tapl, TIP.
- [Alexa VanHattum](https://github.com/avanhatt) - Artifact Evaluation: Kani Rust Verifier (Kani).
- [Pavol Vargovčík](https://github.com/p4l1ly) - z3-rust.
- [Herman Venter](https://github.com/hermanventer) - MIRAI, Rust static analysis/verification reading and resources.
- [Mark Verleg](https://markv.nl) - prover(2).
- [Nathaniel Victor](https://github.com/NVictor2004) - SAT Solver(2).
- [Nikita Voronov](https://orsinium.dev) - RLCI.
- [Shuxian Wang](https://github.com/wsx-ucb) - QED Prover.
- [Max Willsey](https://www.mwillsey.com) - egg, egglog.
- [Ivo Wingelaar](https://github.com/IvoWingelaar) - compiler, mmb-binutils, mmb-parser, mmb-types, The Trivial Metamath Zero kernel, Verifier.
- [Jan Winkelmann](https://github.com/keks) - smtlib-syntax.
- [Florian Würmseer](https://github.com/FWuermse) - SAT-Solver.
- [Jieyou Xu](https://github.com/jieyouxu) - Propositional Tableaux Solver.
- [Ren Yanjie](https://github.com/Rose1917) - bool2dimacs, RustLogic.
- [Brendan Zabarauskas](https://github.com/brendanzab) - Fathom, moniker, Pikelet, rust-nbe-for-mltt.
- [Bas Zalmstra](https://github.com/baszalmstra) - Resolvo.
- [Alexey Zatelepin](https://github.com/ztlpn) - minilp.
- [Eric Zhang](https://www.ekzhang.com) - µKanren-rs.
- [Hanliang Zhang](https://github.com/KomaEc) - sat.
- [Tesla Ice Zhang](https://ice1000.org) - minitt-rs, Narc, Voile.
- [Xie Zhongtao](https://github.com/francisol) - rssat.
- [Felix Zhu](https://github.com/felixzhuologist) - lambdacube.
- [Li Zhuohua](https://zhuohua.me) - MirChecker.
- [Philip Zucker](https://github.com/philzook58) - res-rs.