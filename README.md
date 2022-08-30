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

- Archived :skull:
- Best in Class :diamonds:
- Book implementation :book:
- Crate(s) :package:
- Crates keyword fully listed :100:
- Deleted by author :recycle:
- Exhumated :ghost:
- Inactive :zzz:
- List of resources :information_source:
- Popular :star:
- Research paper implementation :lab_coat:
- Toy project :baby_chick:
- Video :tv:
- WIP :construction:

## Projects

### Provers and Solvers

#### Provers TPTP compliant

- [CoP](https://github.com/01mf02/cop-rs) [:package:](https://crates.io/crates/cop) - reimplement automated theorem provers of the leanCoP family, such as leanCoP and nanoCoP.
- [lazyCoP](https://github.com/MichaelRawson/lazycop) - automatic theorem prover for first-order logic with equality.
- [lerna](https://github.com/MichaelRawson/lerna) :skull: - proves theorems.
- [lickety](https://github.com/MichaelRawson/lickety) - prototype system for linear resolution with splitting.
- [meancop](https://github.com/01mf02/cop-rs) [:package:](https://crates.io/crates/meancop):recycle: - became CoP.
- [Serkr](https://github.com/mAarnos/Serkr) [:ghost:](https://github.com/newca12/Serkr) :star: - automated theorem prover for first order logic with equality.

#### SAT Solver

- [BatSat](https://github.com/c-cube/batsat) [:package:](https://crates.io/crates/batsat):star: - solver forked from ratsat, a reimplementation of MiniSat.
- [CreuSAT](https://github.com/sarsko/CreuSAT) :star: - formally verified SAT solver verified with Creusot.
- [Debug-SAT](https://github.com/advancedresearch/debug_sat) [:package:](https://crates.io/crates/debug_sat) - debuggable automatic theorem prover for boolean satisfiability problems (SAT).
- [dpll-sat](https://github.com/snsinfu/dpll-sat) - naïve SAT solver implementing the classic DPLL algorithm.
- [msat](https://github.com/solhop/msat) [:package:](https://crates.io/crates/msat) - MaxSAT Solver.
- [RatSat](https://github.com/qnighy/ratsat) [:package:](https://crates.io/crates/ratsat)[:package:](https://crates.io/crates/ratsat-bin):star: - reimplementation of MiniSat.
- [rsat](https://github.com/solhop/rsat) [:package:](https://crates.io/crates/rsat) - SAT Solver.
- [rust-smt-ir](https://github.com/awslabs/rust-smt-ir) - provides an intermediate representation (IR) in Rust for SMT-LIB queries along with tools.
- [rustsat](https://github.com/jamesbornholt/rustsat) :baby_chick: - toy Rust SAT solver.
- [SATCoP](https://github.com/MichaelRawson/satcop) - theorem prover for first-order logic based on connection tableau and SAT solving.
- [Satire](https://github.com/Qwaz/satire) [:package:](https://crates.io/crates/satire) - educational SAT solver.
- [SAT-MICRO](https://github.com/OCamlPro/sat_micro_rust) [:lab_coat:](https://hal.inria.fr/inria-00202831/en) - reimplementation of the SAT-solver described in 'SAT-MICRO: petit mais costaud!'.
- [scrapsat](https://github.com/togatoga/scrapsat) :construction: - CDCDL SAT Solver.
- [screwsat](https://github.com/togatoga/screwsat) [:package:](https://crates.io/crates/screwsat):star: - simple CDCL SAT Solver.
- [slp](https://github.com/solhop/slp) [:package:](https://crates.io/crates/slp):recycle: - became SolHOP.
- [SolHOP](https://github.com/solhop/solhop) [:package:](https://crates.io/crates/solhop):skull: - aims to be a SAT and MaxSAT solver. Currently, a CDCL based SAT.
- [Splr](https://github.com/shnarazk/splr) [:package:](https://crates.io/crates/splr):diamonds::star: - modern CDCL SAT solver.
- [starlit](https://github.com/jix/starlit) :construction: - CDCL SAT solver.
- [Stevia](https://github.com/Robbepop/stevia) :star: - simple (unfinished) SMT solver for QF_ABV.
- [UASAT-RS](https://github.com/mmaroti/uasat-rs) - SAT solver based calculator for discrete mathematics and universal algebra.
- [Varisat](https://github.com/jix/varisat)[:package:](https://crates.io/crates/varisat)[:package:](https://crates.io/crates/varisat-checker)[:package:](https://crates.io/crates/varisat-cli)[:package:](https://crates.io/crates/varisat-dimacs)[:package:](https://crates.io/crates/varisat-formula)[:package:](https://crates.io/crates/varisat-internal-macros)[:package:](https://crates.io/crates/varisat-internal-proof)[:package:](https://crates.io/crates/varisat-lrat):star: - CDCL based SAT solver.

#### Proof assistant
- [cobalt](https://github.com/lcnr/cobalt) :recycle:[:ghost:](https://github.com/isgasho/cobalt) - a wip minimal proof assistant.
- [Esther](https://github.com/aodhneine/esther) :construction: - simple automated proof assistant.
- [LSTS](https://github.com/andrew-johnson-4/LSTS) [:package:](https://crates.io/crates/lsts):star: - proof assistant that is also a programming language.
- [Noq](https://github.com/tsoding/Noq) [:tv:](https://www.youtube.com/playlist?list=PLpM-Dvs8t0VZVE64QKPf6y_TIUwj5nKQ7):star: - Not Coq. Simple expression transformer that is not Coq.
- [Poi](https://github.com/advancedresearch/poi) [:package:](https://crates.io/crates/poi):star: - pragmatic point-free theorem prover assistant.
- [qbar](https://github.com/qdeduction/qbar) [:package:](https://crates.io/crates/qbar) - experimental automated theorem verifier/prover and proof assistant.
#### Misc

- [Avalog](https://github.com/advancedresearch/avalog) [:package:](https://crates.io/crates/avalog):star: - experimental implementation of Avatar Logic with a Prolog-like syntax.
- [Caso](https://github.com/advancedresearch/caso) [:package:](https://crates.io/crates/caso) - category Theory Solver for Commutative Diagrams.
- [gpp-solver](https://github.com/Ereski/gpp-solver) [:package:](https://crates.io/crates/gpp-solver) - small hybrid push-pull solver/planner that has the best of both worlds.
- [hoice](https://github.com/hopv/hoice) :star: - ICE-based Constrained Horn Clause (CHC) solver.
- [linear_solver](https://github.com/advancedresearch/linear_solver) [:package:](https://crates.io/crates/linear_solver):star: - linear solver designed to be easy to use with Rust enums.
- [Logic solver](https://github.com/qnighy/logic-solver-rs) :star: - logic solver.
- [Mikino](https://github.com/OCamlPro/mikino) [:package:](https://crates.io/crates/mikino)[:package:](https://crates.io/crates/mikino_api) - simple induction and BMC engine.
- [minilp](https://github.com/ztlpn/minilp) [:package:](https://crates.io/crates/minilp):star: - linear programming solver.
- [Monotonic-Solver](https://github.com/advancedresearch/monotonic_solver) [:package:](https://crates.io/crates/monotonic_solver):star: - monotonic solver designed to be easy to use with Rust enum expressions.
- [pocket_prover](https://github.com/advancedresearch/pocket_prover) [:package:](https://crates.io/crates/pocket_prover)[:package:](https://crates.io/crates/pocket_prover-derive):star: - fast, brute force, automatic theorem prover for first order logic.
- [reachability_solver](https://github.com/advancedresearch/reachability_solver) [:package:](https://crates.io/crates/reachability_solver) - linear reachability solver for directional edges.
- [relsat-rs](https://github.com/mmaroti/relsat-rs) :baby_chick: - Experiments with  provers.
- [shari](https://github.com/nyuichi/shari) - the 🍣 prover.

### Verification

#### Static Analysis & Rust verification tools

- [contracts](https://gitlab.com/karroffel/contracts) [:package:](https://crates.io/crates/contracts):star: - implements "[Design By Contract](https://en.wikipedia.org/wiki/Design_by_contract)" via procedural macros.
- [Creusot](https://github.com/xldenis/creusot) :star: - tool for deductive verification of Rust code.
- [crux-mir](https://github.com/GaloisInc/crucible/tree/master/crux-mir) :star: - static simulator for Rust programs.
- [cwe_checker](https://github.com/fkie-cad/cwe_checker) :star: - finds vulnerable patterns in binary executables.
- [electrolysis](https://github.com/Kha/electrolysis) :star: - tool for formally verifying Rust programs by transpiling them into the Lean 2 theorem prover.
- [Flux](https://github.com/liquid-rust/flux) :star:[:lab_coat:](https://arxiv.org/pdf/2207.04034.pdf) - liquid types for Rust.
- [Kani](https://github.com/model-checking/kani) :star:[:lab_coat:](https://www.cs.cornell.edu/~avh/dyn-trait-icse-seip-2022-preprint.pdf) - bit-precise model-checker, ensures that unsafe Rust code is actually safe.
- [Loom](https://github.com/tokio-rs/loom) [:package:](https://crates.io/crates/loom):star: - concurrency permutation testing tool for Rust.
- [matla](https://github.com/OCamlPro/matla) - a manager for TLA+ projects.
- [MIRAI](https://github.com/facebookexperimental/MIRAI) [:package:](https://crates.io/crates/mirai-annotations):star: - intended to become a widely used static analysis tool for Rust.
- [MirChecker](https://github.com/lizhuohua/rust-mir-checker) :star:[:lab_coat:](https://www.cse.cuhk.edu.hk/~cslui/PUBLICATION/CCS2021.pdf) - simple static analysis tool.
- [p4-analyzer](https://github.com/AzureMarker/p4-analyzer) - static analysis tool which checks P4 code for bugs.
- [Prusti](https://github.com/viperproject/prusti-dev) :star: - prototype verifier for Rust, built upon the the Viper verification infrastructure.
- [Rudra](https://github.com/sslab-gatech/Rudra) :star:[:lab_coat:](https://github.com/sslab-gatech/Rudra/blob/master/rudra-sosp21.pdf) - static analyzer to detect common undefined behaviors in Rust programs.
- [Rust static analysis/verification reading and resources](https://github.com/facebookexperimental/MIRAI/blob/main/documentation/FurtherReading.md) :information_source: - for further reading.
- [Rust verification tools](https://github.com/project-oak/rust-verification-tools) :star: - collection of tools/libraries about static and dynamic verification of Rust programs.
- [Rust verification tools (2021)](https://rust-formal-methods.github.io/tools.html) :information_source: - list of Rust verification tools with a bias towards ‘formal methods’ tools.
- [Rust verification tools list](https://alastairreid.github.io/automatic-rust-verification-tools-2021) :information_source: - list of tools.
- [RustHorn](https://github.com/hopv/rust-horn) [:lab_coat:](https://link.springer.com/chapter/10.1007%2F978-3-030-44914-8_18) - CHC-based Automated Verification Tool for Rust.
- [RustHornBelt Library & Benchmarks](https://github.com/xldenis/rhb-specs) [:lab_coat:](https://zenodo.org/record/6426048) - support paper in preview.
- [Rustproof](https://github.com/Rust-Proof/rustproof) [:package:](https://crates.io/crates/rustproof):star: - compiler plugin, verification condition generator.
- [Shuttle](https://github.com/awslabs/shuttle) [:package:](https://crates.io/crates/shuttle):star: - library for testing concurrent Rust code.
- [Stateright](https://github.com/stateright/stateright) [:package:](https://crates.io/crates/stateright):star: - model checker for implementing distributed systems.
- [VeriWasm](https://github.com/PLSysSec/veriwasm) [:package:](https://crates.io/crates/veriwasm):star:[:lab_coat:](http://cseweb.ucsd.edu/~dstefan/pubs/johnson:2021:veriwasm.pdf) - SFI verifier of Wasm binaries.
- [verus](https://github.com/secure-foundations/verus) :star: - verified subset of Rust for low-level systems code.
- [Xori](https://github.com/endgameinc/xori) :star: - static analysis library for PE32, 32+ and shellcode.

#### Misc

- [ArcsJs - Provable](https://github.com/project-oak/arcsjs-provable) - set of ArcsJs focused tools for doing proofs on ArcsJs models.
- [Bounded Registers](https://github.com/auxoncorp/bounded-registers) [:package:](https://crates.io/crates/bounded-registers):star: - high-assurance memory-mapped register interaction library.
- [Chalk](https://github.com/rust-lang/chalk) [:package:](https://crates.io/crates/chalk-solve)[:package:](https://crates.io/crates/chalk-derive)[:package:](https://crates.io/crates/chalk-engine)[:package:](https://crates.io/crates/chalk-ir)[:package:](https://crates.io/crates/chalk-macros)[:package:](https://crates.io/crates/chalk-recursive)[:package:](https://crates.io/crates/chalk-rust-ir):star: - implements the Rust trait system, based on Prolog-ish logic rules.
- [Charon](https://github.com/sonmarcho/charon) - interface with the rustc compiler for the purpose of program verification.
- [Kinō](https://github.com/kino-mc/kino) :skull: - re-implementation of the core verification engine of [Kind 2 model-checker](https://kind2-mc.github.io/kind2).
- [Kontroli](https://github.com/01mf02/kontroli-rs) [:package:](https://crates.io/crates/dedukti-parse)[:package:](https://crates.io/crates/kocheck)[:package:](https://crates.io/crates/kontroli)[:tv:](https://www.youtube.com/watch?v=lLjWBsU_BX0)[:lab_coat:](https://arxiv.org/pdf/2102.08766.pdf):diamonds: - alternative implementation of the logical framework Dedukti.
- [Metamath-knife](https://github.com/david-a-wheeler/metamath-knife) - verify Metamath proofs.
- [pocket_prover-set](https://github.com/advancedresearch/pocket_prover-set) [:package:](https://crates.io/crates/pocket_prover-set) - base logical system for PocketProver to reason about set properties.
- [rate](https://github.com/krobelus/rate) [:package:](https://crates.io/crates/rate)[:package:](https://crates.io/crates/rate-common)[:package:](https://github.com/krobelus/rate)[:package:](https://crates.io/crates/rate-proof-utils)[:package:](https://crates.io/crates/rate-sick-check):diamonds: - clausal proof checker (DRAT, DPR) for certifying SAT solvers' unsatisfiability results.
- [rlfsc](https://github.com/alex-ozdemir/rlfsc) [:package:](https://crates.io/crates/rlfsc) - checker for the LFSC proof language.
- [second_opinion](https://github.com/ammkrn/second_opinion) - verifier for Metamath Zero proof files.
- [smetamath](https://github.com/sorear/smetamath-rs) [:package:](https://crates.io/crates/smetamath) :star: - parallel and incremental verifier for Metamath databases.
- [Supervisionary](https://github.com/veracruz-project/supervisionary) [:lab_coat:](https://dominicpm.github.io/publications/mulligan-supervisionary-2022.pdf) - experimental proof-checking system for Gordon's higher-order logic.
- [t3p](https://github.com/skbaek/tesc/tree/master/t3p-rs) - optimized TESC (Theory-Extensible Sequent Calculus) verifier.
- [Verifier](https://github.com/trivial-rs/verifier) [:package:](https://crates.io/crates/trivial-verifier) - Trivial proof verifier - an interface to the Metamath Zero kernel.

### Libraries

#### Parser

- [CNF Parser](https://github.com/robbepop/cnf-parser) [:package:](https://crates.io/crates/cnf-parser) - efficient and customizable parser for the .cnf file format.
- [DIMACS Parser](https://github.com/robbepop/dimacs-parser) [:package:](https://crates.io/crates/dimacs) - utilities to parse files in DIMACS .cnf or .sat file format.
- [Flussab CNF](https://github.com/jix/flussab) [:package:](https://crates.io/crates/flussab-cnf) - parsing and writing of the DIMACS CNF file format.
- [FRAT-rs](https://github.com/digama0/frat) [:lab_coat:](https://arxiv.org/pdf/2109.09665.pdf) - toolchain for processing and transforming files in the FRAT format.
- [Lambda Term Parsing](https://github.com/01mf02/lambda-parse) - explores different parser designs for a simple lambda term grammar.
- [mmb-parser](https://github.com/trivial-rs/mmb-parser) [:package:](https://crates.io/crates/mmb-parser) - parser for the Metamath Zero binary proof format.
- [olean-rs](https://github.com/digama0/olean-rs) - parser/viewer for olean files.
- [smt2](https://github.com/regular-pv/smt2) [:package:](https://crates.io/crates/smt2) - SMT-LIB 2 parsing library.
- [tptp](https://github.com/MichaelRawson/tptp) [:package:](https://crates.io/crates/tptp):diamonds: - parse the TPTP format.

#### Bindings

- [boolector](boolector) [:package:](https://crates.io/crates/boolector) - safe high-level bindings for the [Boolector](https://boolector.github.io) SMT solver.
- [bitwuzla-sys](https://github.com/fatemender/bitwuzla-sys) [:package:](https://crates.io/crates/bitwuzla-sys) - low-level bindings for the [Bitwuzla](https://bitwuzla.github.io) SMT solver.
- [boolector-sys](https://github.com/fatemender/boolector-sys) [:package:](https://crates.io/crates/boolector-sys) - low-level bindings for the [Boolector](https://boolector.github.io) SMT solver.
- [CaDiCaL SAT solver](https://github.com/mmaroti/cadical-rs) [:package:](https://crates.io/crates/cadical) - bindings for the CaDiCaL SAT solver.
- [cryptominisat-rs](https://github.com/storyyeller/cryptominisat-rs) [:package:](https://crates.io/crates/cryptominisat) - bindings for [CryptoMiniSat](https://github.com/msoos/cryptominisat).
- [falcon-z3](https://github.com/falconre/falcon-z3) [:package:](https://crates.io/crates/falcon-z3) - bindings for Z3.
- [IPASIR](https://github.com/robbepop/ipasir-rs) [:package:](https://crates.io/crates/ipasir) - FFI bindings for the IPASIR incremental SAT solver interface.
- [Kissat-rs](https://github.com/firefighterduck/kissat-rs) [:package:](https://crates.io/crates/kissat) - bindings for the Kissat SAT solver.
- [lean-sys](https://gitlab.com/tekne/lean-sys) [:package:](https://crates.io/crates/lean-sys) - bindings to Lean 4's C API.
- [libsmt.rs](https://github.com/sushant94/libsmt.rs) - bindings for SMTLIB2.
- [rsmt2](https://github.com/kino-mc/rsmt2) [:package:](https://crates.io/crates/rsmt2)[:package:](https://crates.io/crates/rsmt2-zz):star: - generic library to interact with SMT-LIB 2 compliant solvers.
- [Rust-SMT-LIB-API](https://github.com/facebookarchive/Rust-SMT-LIB-API) [:package:](https://crates.io/crates/rust_smt):skull::star: - generic high-level API for interacting with SMT solvers.
- [rustproof-libsmt](https://github.com/Rust-Proof/libsmt.rs) [:package:](https://crates.io/crates/rustproof-libsmt) - fork of libsmt.rs.
- [z3](https://github.com/prove-rs/z3.rs) [:package:](https://crates.io/crates/z3)[:package:](https://crates.io/crates/z3-sys):star: - high-level and low-level Rust bindings for the Z3 solver.
- [z3-rust](https://github.com/p4l1ly/z3-rust) [:package:](https://crates.io/crates/z3_ref) - high level bindings for the Microsoft's Z3 SMT solver.
- [Z3D](https://github.com/alex-chew/z3d-rs) [:package:](https://crates.io/crates/z3d) - Z3 DSL interface.

#### Translator

- [anthem](https://github.com/potassco/anthem) - translate answer set programs to first-order theorem prover language.
- [Cnfpack](https://github.com/jix/cnfpack) [:package:](https://crates.io/crates/cnfpack) - converts between DIMACS CNF file format and the compressed binary Cnfpack format.
- [hz-to-mm0](https://github.com/digama0/hz-to-mm0) - translator from HOL Zero / Common HOL to Metamath Zero.

#### Misc

- [AbsoluteUnity](https://github.com/ray-kast/AbsoluteUnity) - think Prolog, but less capable.
- [Alice_rs](https://github.com/firefighterduck/alice_rs) [:lab_coat:](http://www0.cs.ucl.ac.uk/staff/p.ohearn/papers/unroll_collapse_withproofs.pdf)[:lab_coat:](https://www21.in.tum.de/teaching/sar/SS20/8.pdf) - implementation of a decision procedure for A Decidable Fragment of Separation Logic.
- [Avatar Hypergraph Rewriting](https://github.com/advancedresearch/avatar_hypergraph_rewriting) [:package:](https://crates.io/crates/avatar_hypergraph_rewriting) - hypergraph rewriting system with avatars for symbolic distinction.
- [coc](https://github.com/azdavis/coc) - the calculus of constructions.
- [compiler](https://github.com/trivial-rs/compiler) [:package:](https://crates.io/crates/trivial-compiler):baby_chick: - trivial compiler framework for Metamath Zero binary proofs.
- [discrimination-tree](https://github.com/MichaelRawson/discrimination-tree) [:package:](https://crates.io/crates/discrimination-tree) - discrimination tree term indexing.
- [egg](https://github.com/egraphs-good/egg) [:package:](https://crates.io/crates/egg):star: - flexible, high-performance e-graph library.
- [epilog](https://github.com/ray-kast/epilog) [:package:](https://crates.io/crates/epilog) - collection of Prolog-like tools for inference logic.
- [FALL](https://github.com/remexre/fall) [:package:](https://crates.io/crates/fall) - easily embeddable, futures-friendly logic engine.
- [Fathom](https://github.com/yeslogic/fathom) [:package:](https://crates.io/crates/fathom):star: - declarative data definition language for formally specifying binary data formats.
- [foliage](https://github.com/potassco/foliage) [:package:](https://crates.io/crates/foliage) - first-order logic with integer arithmetics.
- [Joker Calculus](https://github.com/advancedresearch/joker_calculus.git) [:package:](https://crates.io/crates/joker_calculus) -  implementation of Joker Calculus in Rust.
- [Kravanenn](https://github.com/ppedrot/kravanenn) :star: - set of tools for Coq.
- [LogRu](https://github.com/fatho/logru) [:package:](https://crates.io/crates/logru) - small, embeddable and fast interpreter for a subset of Prolog.
- [mm0-rs](https://github.com/digama0/mm0/tree/master/mm0-rs) [:package:](https://crates.io/crates/mm0b_parser)[:package:](https://crates.io/crates/mm0_deepsize)[:package:](https://crates.io/crates/mm0_util):star:[:lab_coat:](https://digama0.github.io/mm0/thesis-slides.pdf)[:lab_coat:](https://digama0.github.io/mm0/thesis.pdf) - MM0/MM1 server and utilities.
- [mmb-binutils](https://github.com/trivial-rs/mmb-binutils) - utility tools for Metamath Zero binary proof files.
- [mmb-types](https://crates.io/crates/mmb-types) - library containing the definitions of the opcodes in the Metamath Zero binary proof files.
- [moniker](https://github.com/brendanzab/moniker) [:package:](https://crates.io/crates/moniker)[:package:](https://crates.io/crates/moniker-derive):star: - automagical variable binding library. 
- [nanoda](https://github.com/ammkrn/nanoda) :skull::star: - became nanoda-lib.
- [nanoda_lib](https://github.com/ammkrn/nanoda_lib) - type inference/checking functionality based on the Lean theorem prover.
- [polytype](https://github.com/lucasem/polytype-rs) [:package:](https://crates.io/crates/polytype):star: - Hindley-Milner polymorphic typing system.
- [program-induction](https://github.com/lucasem/program-induction) [:package:](https://crates.io/crates/programinduction):star: - library for program induction and learning representations.
- [rust-nbe-for-mltt](https://github.com/brendanzab/rust-nbe-for-mltt) :star: - normalization by evaluation for Martin-Löf Type Theory with dependent records.
- [rust-unify](https://github.com/bongo227/rust-unify) [:package:](https://crates.io/crates/rust-unify) :recycle: - unification algorithum implementation.
- [Rusty Razor](https://github.com/salmans/rusty-razor) [:package:](https://crates.io/crates/razor)[:package:](https://crates.io/crates/razor-fol)[:package:](https://crates.io/crates/razor-chase):star: - tool for constructing finite models for first-order theories.
- [Satoxid](https://github.com/neuring/satoxid) [:package:](https://crates.io/crates/satoxid) - library to help with encoding SAT problems.
- [smt2utils](https://github.com/facebookincubator/smt2utils) [:package:](https://crates.io/crates/smt2parser)[:package:](https://crates.io/crates/smt2patch)[:package:](https://crates.io/crates/smt2proxy)[:package:](https://crates.io/crates/z3tracer) - libraries and tools for the SMT-LIB-2 standard.
- [term-rewriting-rs](https://github.com/joshrule/term-rewriting-rs) [:package:](https://crates.io/crates/term_rewriting) :star: - representing, parsing, and computing with first-order term rewriting systems.
- [tribool](https://github.com/novacrazy/rust-tribool) [:package:](https://crates.io/crates/tribool) - three-valued logic.
- [The Trivial Metamath Zero kernel](https://github.com/trivial-rs/kernel) [:package:](https://crates.io/crates/trivial-kernel) - Metamath Zero kernel for Trivial.
- [Whisper](https://github.com/sdleffler/whisper) :star: - logic Programming DSL.

## Books code

*There is [numerous](https://github.com/search?l=Rust&q=tapl&type=Repositories) implementations of TAPL [:book:](https://www.cis.upenn.edu/~bcpierce/tapl), we keep only the most popular and keep an eye on implementations that worth attention.*

- [logic-rs](https://github.com/ixjf/logic-rs) [:book:](https://ruccs.rutgers.edu/lepore-meaning-and-argument/lepore-about-the-book):skull::star: - parser of relational predicate logic & truth tree solver
- [plar-rs](https://github.com/nikomatsakis/plar-rs) [:book:](https://www.cl.cam.ac.uk/~jrh13/atp)[:ghost:](https://github.com/newca12/plar-rs) - exploring John Harrison's Handbook of Practical Logic and Automated Reasoning.
- [tapl](https://github.com/v4kst1z/tapl) - implementation of TAPL.
- [TAPL in Rust](https://github.com/hayatoito/tapl-in-rust) :star: - another collection of implementations of TAPL.
- [tnt](https://github.com/SymmetricChaos/tnt) [:book:](https://en.wikipedia.org/wiki/G%C3%B6del,_Escher,_Bach)[:package:](https://crates.io/crates/tnt) - implementation of Hofstader's "Typographical Number Theory" from the book Gödel, Escher & Bach.
- [types-and-programming-languages](https://github.com/lazear/types-and-programming-languages) :star: - Exercises from Benjamin Pierce's TAPL textbook + extras!

## Programming Language

- [egglog](https://github.com/philzook58/egglog) :star: - using the egg library with a file format and semantics similar to datalog.
- [High-order Virtual Machine (HVM)](https://github.com/Kindelia/HVM) :star: - massively parallel, optimal functional runtime.
- [isotope-prover-experiments](https://gitlab.com/isotope-project/isotope-prover-experiments) :construction: [:lab_coat:](https://gitlab.com/tekne/phd-proposal/-/blob/main/report.tex) [:lab_coat:](https://gitlab.com/isotope-project/msc-thesis/-/blob/master/thesis.tex) - experimental dependently typed language supporting borrow checking.
- [Kind2](https://github.com/Kindelia/Kind2) [:package:](https://crates.io/crates/kind2):star: - modern proof language prototype successor of [Kind-Lang](https://github.com/kindelia/kind).
- [Last Order Logic](https://github.com/advancedresearch/last_order_logic.git) [:package:](https://crates.io/crates/last_order_logic) - experimental logical language.
- [minihl](https://github.com/firefighterduck/minihl) - formal methods playgorund for MiniHeapLang language.
- [minitt-rs](https://github.com/owo-lang/minitt-rs) [:package:](https://crates.io/crates/minitt)[:package:](https://crates.io/crates/minitt-util):skull::star: - became Voile.
- [Narc](https://github.com/owo-lang/narc-rs) [:package:](https://crates.io/crates/nar):star: - dependently-typed programming language with Agda style dependent pattern matching.
- [Pikelet](https://github.com/pikelet-lang/pikelet) [:package:](https://crates.io/crates/pikelet):star: - small, functional, dependently typed programming language.
- [proto-vulcan](https://github.com/terohuttunen/proto-vulcan) [:package:](https://crates.io/crates/proto-vulcan)[:package:](https://crates.io/crates/proto-vulcan-macros) - miniKanren-family relational logic programming language.
- [Scryer Prolog](https://github.com/mthom/scryer-prolog) [:package:](https://crates.io/crates/scryer-prolog):star: - modern Prolog implementation.
- [Symmetric Interaction Calculus](https://github.com/maiavictor/symmetric-interaction-calculus) :star: - match the optimal λ-calculus reduction algorithm perfectly.
- [tako](https://github.com/Cypher1/tako) -  experimental programming language for ergonomic software verification.
- [TIP](https://github.com/v4kst1z/TIP) :baby_chick: - imperative programming language aimed at teaching fundamental concepts of static program analysis.
- [Untyped Concatenative Calculus](https://github.com/dawn-lang/ucc) - toy programming language and prototype for [Dawn](https://www.dawn-lang.org).
- [Voile](https://github.com/owo-lang/voile-rs) [:package:](https://crates.io/crates/voile)[:package:](https://crates.io/crates/voile-util):skull::star: - became Narc.
- [zz](https://github.com/zetzit/zz) [:package:](https://crates.io/crates/zz):skull::star: - zymbolic verifier and tranzpiler to bare metal C.

## Kanren

- [Canrun](https://github.com/tgecho/canrun_rs) [:package:](https://crates.io/crates/canrun):star: - logic programming library inspired by the *Kanren family of language DSLs.
- [miniKANREN](https://github.com/mbillingr/miniKANREN) [:package:](https://crates.io/crates/mini-kanren) - miniKANREN as a DSL.
- [rslogic](https://github.com/kulibali/rslogic) [:package:](https://crates.io/crates/rslogic):star: - logic programming framework for Rust inspired by µKanren.
- [rust-kanren](https://github.com/wartmanm/rust-kanren) :star: - loose interpretation of miniKanren and cKanren.
- [µKanren-rs](https://github.com/ekzhang/ukanren-rs) [:package:](https://crates.io/crates/ukanren):star: - implementation of µKanren.

## Lambda Calculus

- [blc](https://github.com/ljedrz/blc) [:package:](https://crates.io/crates/blc) - implementation of the binary lambda calculus.
- [Closure Calculus](https://github.com/advancedresearch/closure_calculus) [:package:](https://crates.io/crates/closure_calculus)[:lab_coat:](https://dl.acm.org/doi/abs/10.1145/3294032.3294085) - library for Barry Jay's Closure Calculus.
- [lambda_calc](https://gitlab.com/mcmfb/lambda-calculator) [:package:](https://crates.io/crates/lambda_calc) - command-line untyped lambda calculus interpreter.
- [lambda_calculus](https://github.com/ljedrz/lambda_calculus) [:package:](https://crates.io/crates/lambda_calculus):star: - simple, zero-dependency implementation of pure lambda calculus in safe Rust.
- [lambda_calculus](https://github.com/thomasdziedzic/lambda_calculus) - no description.
- [lambdacube](https://github.com/felixzhuologist/lambdacube) :construction: - implementation of the lambda cube (and other type stuff).
- [Lamcal](https://github.com/haraldmaida/lamcal) [:package:](https://crates.io/crates/lamcal)[:package:](https://crates.io/crates/lamcal-repl) - lambda calculus parser and evaluator and a separate command line REPL.

## Propositional logic
- [Chevre](https://github.com/pvdrz/chevre) :recycle: - small propositional logic interpreter.
- [logic](https://github.com/nextzhou/logic) [:package:](https://crates.io/crates/logic) :baby_chick: - crate for propositional logic.
- [logic-resolver](https://github.com/gustafla/logic-resolver) :baby_chick: - toy implementation of resolution for propositional logic.
- [plc](https://github.com/trolleyman/plc) - propositional logic calculator.
- [Prop](https://github.com/advancedresearch/prop) [:package:](https://crates.io/crates/prop) - library for theorem proving with Intuitionistic Propositional Logic.
- [Propositional Tableaux Solver](https://github.com/jieyouxu/propositional-tableau-solver-rs) [:package:](https://crates.io/crates/propositional-tableau-solver-rs) - solver using the propositional tableaux method.
- [Resolution Prover](https://github.com/ExcaliburZero/resolution-prover) - resolution prover library for propositional logic.
- [rs-logik](https://github.com/SolarLiner/rs-logik) [:ghost:](https://github.com/newca12/rs-logik) - propositional logic interpreter.
- [rusty-logic](https://github.com/mcheatham/rusty-logic) :baby_chick: - propositional logic analysis.
- [simple-proof-assistant](https://github.com/long-long-float/simple-proof-assistant) :baby_chick: - a proof assistant kernel for minimal propositional logic.
- [validator](https://github.com/Maaarcocr/validator) - small utility to test a propositional logic theorem prover.

## Unclassified

- [formal-systems-learning-rs](https://github.com/joshrule/formal-systems-learning-rs) - simulations to learn formal systems as typed first-order term rewriting systems.
- [list-routine-learning-rs](https://github.com/joshrule/list-routine-learning-rs) - simulations to learn typed first-order term rewriting systems that perform list routines.
- [Minimal models](https://github.com/jix/minimal_models_example) - uses a SAT solver to find minimal partial assignments that are model of a CNF formula.
- [n-queens-sat](https://github.com/erohkohl/n-queens-sat) - modelling n-queens problem as conjunctive normal form and solving it with DPLL algorithm.
- [nonogrid](https://github.com/tsionyx/nonogrid) [:package:](https://crates.io/crates/nonogrid) - lightning fast nonogram solver.
- [rummy_to_sat ](https://github.com/neuring/rummy_to_sat) - implementation of a solver for [Rummy](https://en.wikipedia.org/wiki/Rummy).
- [sudoku_sat](https://github.com/shnarazk/sudoku_sat) - solve Sudoku variants with SAT solvers.
- [Supermux](https://github.com/tuzz/supermux) - reduction of the superpermutation problem to Quantified Boolean Formula.
- [Supersat](https://github.com/tuzz/supersat) - attempt to find superpermutations by reducing the problem to SAT.
- [tarpit-rs](https://github.com/sdleffler/tarpit-rs) :star: - type-level implementation of Smallfuck in Rust. Turing-completeness proof for Rust's type system.

## Resources

### Books

- [Verification for Dummies: SMT and Induction](https://ocamlpro.github.io/verification_for_dummies) - broadly discusses induction as a formal verification technique.

### Research Paper & Thesis

- [Hardware/Software Co-Assurance using the Rust Programming Language and ACL2](https://arxiv.org/abs/2205.11709v1) - 2022.
- [Extensible Functional-Correctness Verification of Rust Programs by the Technique of Prophecy](https://github.com/shiatsumat/master-thesis) - 2021.
- [Understanding and Evolving the Rust Programming Language](https://www.ralfj.de/research/thesis.html) - 2020.
- [Simple Verification of Rust Programs via Functional Purification](https://pp.ipd.kit.edu/uploads/publikationen/ullrich16masterarbeit.pdf) - 2016.

### Demos
- [Artifact Evaluation: Kani Rust Verifier](https://github.com/avanhatt/icse22ae-kani) [:lab_coat:](https://www.cs.cornell.edu/~avh/dyn-trait-icse-seip-2022-preprint.pdf) - Kani Rust Model Checker artifact for ICSE 2022 Artifact Evaluation.
- [flux-demo](https://github.com/liquid-rust/flux-demo) - small examples that demonstrate how flux works.

### Blogs

- [A Formal Verification of Rust's Binary Search Implementation.](https://kha.github.io) :uk:
- [Kani Rust Verifier Blog](https://model-checking.github.io/kani-verifier-blog) :uk:
- [Splr notebook.](https://shnarazk.github.io/tag/splr) :jp:
- [Research notebook about improving with Rust the performance of nonclausal automated theorem provers.](https://github.com/01mf02/adam-notes) :uk::diamonds:
- [Articles about a collection of tools/libraries to support both static and dynamic verification of Rust programs.](https://project-oak.github.io/rust-verification-tools) :uk:
- [Varisat notebook.](https://jix.one/blog/rust) :uk:

### Posts

- [Formally Verifying Rust's Opaque Types](https://dylanj.xyz/posts/rust-coq-opaque-types)
- [Solving The Witness with Z3](https://www.techofnote.com/witness-part-1)

### Crates keywords

- [solver](https://crates.io/keywords/solver) - 81 entries. :100:
- [logic](https://crates.io/keywords/logic) - 41 entries. :100:
- [verification](https://crates.io/keywords/verification) - 27 entries. :100:
- [sat](https://crates.io/keywords/sat) - 26 entries. :100:
- [smt](https://crates.io/keywords/smt) - 26 entries. :100:
- [satisfiability](https://crates.io/keywords/satisfiability) - 23 entries. :100:
- [linear-programming](https://crates.io/keywords/linear-programming) - 11 entries.
- [rewriting](https://crates.io/keywords/rewriting) - 8 entries. :100:
- [prover](https://crates.io/keywords/prover) - 8 entries. :100:
- [first-order](https://crates.io/keywords/first-order) - 6 entries. :100:
- [cnf](https://crates.io/keywords/cnf) - 6 entries. :100:
- [smt-lib](https://crates.io/keywords/smt-lib) - 6 entries. :100:
- [metamath-zero](https://crates.io/keywords/metamath-zero) - 5 entries. :100:
- [z3](https://crates.io/keywords/z3) - 5 entries. :100:
- [dependent-types](https://crates.io/keywords/dependent-types) - 5 entries. :100:
- [dimacs](https://crates.io/keywords/dimacs) - 5 entries. :100:

### Community

- [Johannes Altmanninger](https://github.com/krobelus) - rate.
- [Mikko Aarnos](https://github.com/mAarnos) - Serkr.
- [ammkrn](https://twitter.com/ammkrn) - nanoda, nanoda_lib, second_opinion.
- [Yechan Bae](https://qwaz.github.io) - Rudra, Satire.
- [Clark Barrett](https://github.com/cbarrettfb) - Rust-SMT-LIB-API.
- [Mathieu Baudet](https://github.com/ma2bd) - smt2utils.
- [James Bornholt](https://www.cs.utexas.edu/~bornholt) - rustsat, Shuttle.
- [Bickio O'Callahan](https://github.com/Bickio) - Solving The Witness with Z3.
- [Mario Carneiro](https://www.cmu.edu/dietrich/philosophy/people/phd/mario-carneiro.html) - FRAT-rs, hz-to-mm0, mm0-rs, olean-rs, smetamath.
- [Adrien Champion](https://github.com/AdrienChampion) - hoice, Kinō, matla, Mikino, rsmt2, SAT-MICRO, Verification for Dummies.
- [Michelle Cheatham](https://github.com/mcheatham) -  rusty-logic.
- [Alex Chew](https://github.com/alex-chew) - Z3D.
- [Simon Cruanes](https://simon.cedeela.fr) - BatSat.
- [Ariel Davis](https://azdavis.net) - coc.
- [Xavier Denis](https://www.lri.fr/membre_en.php?mb=2819) - Creusot, RustHornBelt Library & Benchmarks, Rust verification tools (2021).
- [Sushant Dinesh](https://github.com/sushant94) - libsmt.rs.
- [Craig Disselkoen](https://cseweb.ucsd.edu/~cdisselk) - boolector.
- [Mark Drobnak](https://github.com/AzureMarker) - p4-analyzer.
- [Bruno Dutertre](https://github.com/BrunoDutertre) - rust-smt-ir.
- [Thomas Dziedzic](https://www.thomasdziedzic0.com) - lambda_calculus.
- [endeav0r](https://github.com/endeav0r) - falcon-z3.
- [Enkelmann](https://github.com/Enkelmann) - cwe_checker.
- [Aodhnait Étaín](https://aodhneine.github.io) - Esther.
- [Michael Färber](http://cl-informatik.uibk.ac.at/users/mfaerber) - CoP, Kontroli, Lambda Term Parsing, meancop, research notebook about improving with Rust the performance of nonclausal automated theorem provers.
- [FireFighterDuck](https://github.com/firefighterduck) - Alice_rs, Kissat-rs, minihl.
- [Robin Freyler](https://robbepop.github.io) - CNF Parser, DIMACS Parser, Stevia.
- [Galois, Inc.](http://galois.com) - crux-mir.
- [Jad Ghalayini](https://gitlab.com/tekne) - isotope-prover-experiments, lean-sys.
- [Nathan Graule ](https://github.com/SolarLiner) - rs-logik.
- [Brandon H. Gomes](https://github.com/bhgomes) - qbar.
- [Robert Grosse](https://github.com/Storyyeller) - cryptominisat-rs.
- [Masaki Hara](https://twitter.com/qnighy) - Logic solver, RatSat.
- [Jannis Harder](https://jix.one) - Cnfpack, Flussab CNF, Minimal models, starlit, Varisat, Varisat notebook.
- [David S. Hardin](https://github.com/david-s-hardin) - Hardware/Software Co-Assurance using the Rust Programming Language and ACL2.
- [Timothée Haudebourg](https://github.com/timothee-haudebourg) - smt2.
- [Son HO](https://github.com/sonmarcho) - Charon.
- [Sarek Høverstad Skotåm](https://github.com/sarsko) - CreuSAT.
- [Tero Huttunen](https://github.com/terohuttunen) - proto-vulcan.
- [Ranjit Jhala](https://github.com/ranjitjhala) - flux-demo.
- [Andrew Johnson](https://github.com/andrew-johnson-4) - LSTS.
- [Evan Johnson](https://github.com/enjhnsn2) - VeriWasm.
- [Dylan R. Johnston](https://dylanj.xyz) - Formally Verifying Rust's Opaque Types.
- [Ralf Jung](https://www.ralfj.de) - Understanding and Evolving the Rust Programming Language.
- [karroffel](https://gitlab.com/karroffel) - contracts.
- [Prateek Kumar](https://prateekkumar.in) - msat, rsat, slp, SolHOP.
- [Alexey Kutepov](https://tsoding.org) - Noq.
- [Ivan Ladelshchikov](https://github.com/tsionyx) - nonogrid.
- [Andrea Lattuada](https://github.com/utaal) - verus.
- [lcnr](https://lcnr.de) - cobalt.
- [Shea Leffler](http://loud.fyi) - tarpit-rs, whisper.
- [Nico Lehmann](https://github.com/nilehmann) - Flux.
- [Carl Lerche](https://github.com/carllerche) - Loom.
- [ljedrz](https://github.com/ljedrz) - blc, lambda_calculus.
- [Patrick Lühne](https://www.luehne.de) - anthem, foliage.
- [Michael Madden](https://github.com/mikemadden42) - Xori.
- [Scott J Maddox](https://github.com/scottjmaddox) - Untyped Concatenative Calculus.
- [Harald Maida](https://github.com/haraldmaida) - Lamcal.
- [Miklos Maroti](https://www.math.u-szeged.hu/~mmaroti) - cadical-rs, relsat-rs, uasat-rs.
- [Niko Matsakis](http://smallcultfollowing.com/babysteps) - Chalk, Kani, plar-rs.
- [Yusuke Matsushita](https://github.com/shiatsumat) - Extensible Functional-Correctness Verification of Rust Programs by the Technique of Prophecy, RustHorn.
- [mcmfb](https://github.com/mcmfb) - lambda_calc.
- [Bruce Mitchener](https://github.com/waywardmonkeys) - z3.
- [Lucas Morales](https://lucasem.com) - polytype, program-induction.
- [Dominic Mulligan](https://dominicpm.github.io) - Supervisionary.
- [Jon Nadal](https://github.com/jonnadal) - Stateright.
- [neuring](https://github.com/neuring) - rummy_to_sat, Satoxid.
- [Sven Nilsen](https://twitter.com/bvssvni) - Avalog, Avatar Hypergraph Rewriting, Caso, Debug-SAT, Joker Calculus, Last Order Logic, linear_solver, Monotonic-Solver, pocket_prover, pocket_prover-set, Poi, Prop, reachability_solver.
- [Yuichi Nishiwaki](http://hagi.is.s.u-tokyo.ac.jp/~yuichi) - shari.
- [Alex Ozdemir](https://cs.stanford.edu/~aozdemir) - rlfsc.
- [Chris Patuzzo](https://tuzz.tech) - Supermux, Supersat.
- [Pierre-Marie Pédrot](https://www.pédrot.fr) - Kravanenn.
- [Arvid E. Picciani](https://github.com/aep) - zz.
- [Dan Pittman](https://dpitt.me) - Bounded Registers.
- [Christian Poveda](https://github.com/pvdrz) - Chevre.
- [Joshua Pratt](https://blog.mimir.systems) - ArcsJs - Provable, tako.
- [Michael Rawson](http://rawsons.uk/michael) - discrimination-tree, lazyCoP, lerna, lickety, SATCoP, tptp.
- [Alastair Reid](https://alastairreid.github.io) - Articles about a collection of tools/libraries to support both static and dynamic verification of Rust programs,Rust verification tools ,Rust verification tools list.
- [Nathan Ringo](https://remexre.xyz) - FALL.
- [Erik Rohkohl](https://blogs.itemis.com/author/erik-rohkohl) - n-queens-sat.
- [Marco Concetto Rudilosso](https://github.com/Maaarcocr) - validator.
- [Josh Rule](http://www.joshrule.com) - formal-systems-learning-rs, list-routine-learning-rs, term-rewriting-rs. 
- [Salman Saghafi](https://github.com/salmans) - Rusty Razor.
- [Michael Salter](https://github.com/salterm) - Rustproof, rustproof-libsmt.
- [Ryan Schroeder](https://ryan-s.net) - AbsoluteUnity, epilog.
- [Carol Schulze](https://github.com/Ereski) - gpp-solver.
- [skbaek](https://github.com/skbaek) - t3p.
- [Narazaki Shuji](https://shnarazk.github.io) - Splr, Splr notebook, sudoku_sat.
- [snsinfu](https://github.com/snsinfu) - dpll-sat.
- [Mikhail Solovev](https://github.com/fatemender) - bitwuzla-sys, boolector-sys.
- [SymmetricChaos](https://github.com/SymmetricChaos) - tnt.
- [Victor Taelin](https://medium.com/@maiavictor) - High-order Virtual Machine (HVM), Kind2, Symmetric Interaction Calculus..
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
- [David A. Wheeler](https://dwheeler.com) - Metamath-knife.
- [Max Willsey](https://www.mwillsey.com) - egg.
- [Ivo Wingelaar](https://github.com/IvoWingelaar) - compiler, mmb-binutils, mmb-parser, mmb-types, The Trivial Metamath Zero kernel, Verifier.
- [Jieyou Xu](https://github.com/jieyouxu) - Propositional Tableaux Solver.
- [Brendan Zabarauskas](https://github.com/brendanzab) - Fathom, moniker, Pikelet, rust-nbe-for-mltt.
- [Alexey Zatelepin](https://github.com/ztlpn) - minilp.
- [Eric Zhang](https://www.ekzhang.com) - µKanren-rs.
- [Tesla Ice Zhang](https://ice1000.org) - minitt-rs, Narc, Voile.
- [Felix Zhu](https://github.com/felixzhuologist) - lambdacube.
- [Li Zhuohua](https://zhuohua.me) - MirChecker.
- [Philip Zucker](http://www.philipzucker.com) - egglog.