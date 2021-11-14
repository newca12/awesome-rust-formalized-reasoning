## About ##
An exhaustive list of all Rust resources regarding automated or semi-automated formalization efforts in any area, constructive mathematics, formal algorithms, and program verification.

awesome-rust-formalized-reasoning is an EDLA project.

The purpose of [edla.org](http://www.edla.org) is to promote the state of the art in various domains.


## Contents

- [Projects](#projects)
  - [Provers & Solvers](#provers-and-solvers)
    - [Provers TPTP compliant](#provers-tptp-compliant)
    - [SAT Solver](#sat-solver)
    - [Misc](#misc)
  - [Verification](#verification)
    - [Static Analysis](#static-analysis)
    - [Cryptographic](#cryptographic)
    - [Misc](#misc)
  - [Libraries](#libraries)
    - [Parser](#parser)
    - [Bindings](#bindings)
    - [Translator](#translator)
    - [Misc](#misc)
  - [Books code](#books-code)
  - [Programming Language](#programming-language)
  - [Kanren](#kanren)
  - [Lambda Calculus](#lambda-calculus)
  - [Unclassified](#unclassified)
- [Resources](#resources)
  - [Books](#books)
  - [Crates keywords](#crates-keywords)
  - [Thesis](#thesis)
  - [Blogs](#blogs)
  - [Community](#community)

---

## Legend

- Abandoned :skull:
- Best in Class :diamonds:
- Book implementation :book:
- Crate(s) :package:
- Deleted :recycle:
- Exhumated :ghost:
- List of resources :information_source:
- Popular :star:
- Research paper implementation :lab_coat:
- Toy project :baby_chick:
- WIP :construction:

## Projects

### Provers and Solvers

#### Provers TPTP compliant

- [CoP](https://github.com/01mf02/cop-rs) [:package:](https://crates.io/crates/cop) - reimplement in Rust several automated theorem provers of the leanCoP family, such as leanCoP and nanoCoP.
- [lazyCoP](https://github.com/MichaelRawson/lazycop) - automatic theorem prover for first-order logic with equality.
- [lerna](https://github.com/MichaelRawson/lerna) :skull: - proves theorems.
- [meancop](https://github.com/01mf02/cop-rs) [:package:](https://crates.io/crates/meancop):skull: - became CoP.
- [Serkr](https://github.com/mAarnos/Serkr) [:ghost:](https://github.com/newca12/Serkr) :star: - automated theorem prover for first order logic with equality.

#### SAT Solver

- [BatSat](https://github.com/c-cube/batsat) [:package:](https://crates.io/crates/batsat):star: - solver forked from ratsat, a reimplementation of MiniSat.
- [Debug-SAT](https://github.com/advancedresearch/debug_sat) [:package:](https://crates.io/crates/debug_sat) - debuggable automatic theorem prover for boolean satisfiability problems (SAT).
- [msat](https://github.com/solhop/msat) [:package:](https://crates.io/crates/msat) - MaxSAT Solver.
- [RatSat](https://github.com/qnighy/ratsat) [:package:](https://crates.io/crates/ratsat)[:package:](https://crates.io/crates/ratsat-bin):star: - reimplementation of MiniSat.- [rsat](https://github.com/solhop/rsat) [:package:](https://crates.io/crates/rsat) - SAT Solver.
- [SATCoP](https://github.com/MichaelRawson/satcop) - theorem prover for first-order logic based on connection tableau and SAT solving.
- [Satire](https://github.com/Qwaz/satire) [:package:](https://crates.io/crates/satire) - educational SAT solver.
- [SAT-MICRO](https://github.com/OCamlPro/sat_micro_rust) - reimplementation of the SAT-solver described in SAT-MICRO: petit mais costaud! by Sylvain Conchon et al.
- [screwsat](https://github.com/togatoga/screwsat) [:package:](https://crates.io/crates/screwsat):star: - simple CDCL SAT Solver.
- [slp](https://github.com/solhop/slp) [:package:](https://crates.io/crates/slp):skull: - became SolHOP.
- [SolHOP](https://github.com/solhop/solhop) [:package:](https://crates.io/crates/solhop) - aims to be a SAT and MaxSAT solver. Currently, a CDCL based SAT.
- [Splr](https://github.com/shnarazk/splr) [:package:](https://crates.io/crates/splr):diamonds::star: - modern CDCL SAT solver.
- [starlit](https://github.com/jix/starlit) :construction: - CDCL SAT solver.
- [UASAT-RS](https://github.com/mmaroti/uasat-rs) - SAT solver based calculator for discrete mathematics and universal algebra.
- [Varisat](https://github.com/jix/varisat)[:package:](https://crates.io/crates/varisat)[:package:](https://crates.io/crates/varisat-checker)[:package:](https://crates.io/crates/varisat-cli)[:package:](https://crates.io/crates/varisat-dimacs)[:package:](https://crates.io/crates/varisat-formula)[:package:](https://crates.io/crates/varisat-internal-macros)[:package:](https://crates.io/crates/varisat-internal-proof)[:package:](https://crates.io/crates/varisat-lrat):star: - CDCL based SAT solver.

#### Misc

- [Avalog](https://github.com/advancedresearch/avalog) [:package:](https://crates.io/crates/avalog):star: - experimental implementation of Avatar Logic with a Prolog-like syntax.
- [Chevre](https://github.com/pvdrz/chevre) :recycle: - small propositional logic interpreter.
- [hoice](https://github.com/hopv/hoice) :star: - ICE-based Constrained Horn Clause (CHC) solver.
- [lapjv](https://github.com/Antti/lapjv-rust) [:package:](https://crates.io/crates/lapjv) - linear Assignmment Problem solver using Jonker-Volgenant algorithm.
- [Logic solver](https://github.com/qnighy/logic-solver-rs) :star: - logic solver.
- [Mikino](https://github.com/OCamlPro/mikino) [:package:](https://crates.io/crates/mikino)[:package:](https://crates.io/crates/mikino_api) - simple induction and BMC engine.
- [Monotonic-Solver](https://github.com/advancedresearch/monotonic_solver) [:package:](https://crates.io/crates/monotonic_solver):star: - monotonic solver designed to be easy to use with Rust enum expressions.
- [pocket_prover](https://github.com/advancedresearch/pocket_prover) [:package:](https://crates.io/crates/pocket_prover)[:package:](https://crates.io/crates/pocket_prover-derive):star: - fast, brute force, automatic theorem prover for first order logic.
- [Poi](https://github.com/advancedresearch/poi) [:package:](https://crates.io/crates/poi):star: - pragmatic point-free theorem prover assistant.
- [Propositional Tableaux Solver](https://github.com/jieyouxu/propositional-tableau-solver-rs) [:package:](https://crates.io/crates/propositional-tableau-solver-rs) - little propositional formula satisfiability solver using the propositional tableaux method.
- [reachability_solver](https://github.com/advancedresearch/reachability_solver) [:package:](https://crates.io/crates/reachability_solver) - linear reachability solver for directional edges.
- [Resolution Prover](https://github.com/ExcaliburZero/resolution-prover) - resolution prover library for propositional logic.
- [shari](https://github.com/nyuichi/shari) - the 🍣 prover.

### Verification

#### Static Analysis

- [Creusot](https://github.com/xldenis/creusot) :star: - tool for deductive verification of Rust code.
- [crux-mir](https://github.com/GaloisInc/crucible/tree/master/crux-mir) :star: - static simulator for Rust programs. It runs a set of test cases and attempts to prove that all assertions pass on all valid inputs.
- [electrolysis](https://github.com/Kha/electrolysis) :star: - tool for formally verifying Rust programs by transpiling them into definitions in the Lean 2 theorem prover.
- [p4-analyzer](https://github.com/AzureMarker/p4-analyzer) - static analysis tool which checks P4 code for bugs.
- [MirChecker](https://github.com/lizhuohua/rust-mir-checker) :star:[:lab_coat:](https://www.cse.cuhk.edu.hk/~cslui/PUBLICATION/CCS2021.pdf) - simple static analysis tool.
- [Rudra](https://github.com/sslab-gatech/Rudra) :star:[:lab_coat:](https://github.com/sslab-gatech/Rudra/blob/master/rudra-sosp21.pdf) - static analyzer to detect common undefined behaviors in Rust programs.
- [Rust verification tools list](https://alastairreid.github.io/automatic-rust-verification-tools-2021/) :information_source: - list of tools.
- [RustHorn](https://github.com/hopv/rust-horn) [:lab_coat:](https://link.springer.com/chapter/10.1007%2F978-3-030-44914-8_18) - CHC-based Automated Verification Tool for Rust.
- [Rustproof](https://github.com/Rust-Proof/rustproof) [:package:](https://crates.io/crates/rustproof):star: - compiler plugin, verification condition generator.
- [TIP](https://github.com/v4kst1z/TIP) :baby_chick: - tiny imperative programming language aimed at teaching the fundamental concepts of static program analysis.
- [VeriWasm](https://github.com/PLSysSec/veriwasm) [:package:](https://crates.io/crates/veriwasm):star:[:lab_coat:](http://cseweb.ucsd.edu/~dstefan/pubs/johnson:2021:veriwasm.pdf) - SFI verifier of Wasm binaries.

#### Cryptographic

- [Nova](https://github.com/Microsoft/Nova) [:package:](https://crates.io/crates/nova-snark):star: - high-speed recursive SNARK (a SNARK proof system.
- [OpenZKP Stark](https://github.com/0xProject/OpenZKP/tree/master/crypto/stark) [:package:](https://crates.io/crates/zkp-stark):star: - implementation of STARK zero-knowledge-proofs.
- [Spartan](https://github.com/microsoft/Spartan) [:package:](https://crates.io/crates/spartan):star: - high-speed zero-knowledge proof system.
- [Winterfell](https://github.com/novifinancial/winterfell) [:package:](https://crates.io/crates/winter-air)[:package:](https://crates.io/crates/winter-crypto)[:package:](https://crates.io/crates/winterfell)[:package:](https://crates.io/crates/winter-fri)[:package:](https://crates.io/crates/winter-math)[:package:](https://crates.io/crates/winter-prover)[:package:](https://crates.io/crates/winter-utils)[:package:](https://crates.io/crates/winter-verifier):star: - a STARK prover and verifier for arbitrary computations.

#### Misc

- [Bounded Registers](https://github.com/auxoncorp/bounded-registers) [:package:](https://crates.io/crates/bounded-registers):star: - high-assurance memory-mapped register interaction library.
- [Chalk](https://github.com/rust-lang/chalk) [:package:](https://crates.io/crates/chalk-solve)[:package:](https://crates.io/crates/chalk-derive)[:package:](https://crates.io/crates/chalk-engine)[:package:](https://crates.io/crates/chalk-ir)[:package:](https://crates.io/crates/chalk-macros)[:package:](https://crates.io/crates/chalk-recursive)[:package:](https://crates.io/crates/chalk-rust-ir):star: - implements the Rust trait system, based on Prolog-ish logic rules.
- [frat-rs](https://github.com/digama0/frat) - verify DIMACS proof.
- [Kinō](https://github.com/kino-mc/kino) :skull: - re-implementation of the core verification engine of [Kind 2 model-checker](https://kind2-mc.github.io/kind2/).
- [Kontroli](https://github.com/01mf02/kontroli-rs)  [:package:](https://crates.io/crates/dedukti-parse)[:package:](https://crates.io/crates/kocheck)[:package:](https://crates.io/crates/kontroli) - alternative implementation of the logical framework Dedukti, concentrating on the verification of proofs.
- [pocket_prover-set](https://github.com/advancedresearch/pocket_prover-set) [:package:](https://crates.io/crates/pocket_prover-set) - base logical system for PocketProver to reason about set properties.
- [Prusti](https://github.com/viperproject/prusti-dev) :star: - prototype verifier for Rust, built upon the the Viper verification infrastructure.
- [rate](https://github.com/krobelus/rate) [:package:](https://crates.io/crates/rate)[:package:](https://crates.io/crates/rate-common)[:package:](https://github.com/krobelus/rate)[:package:](https://crates.io/crates/rate-proof-utils)[:package:](https://crates.io/crates/rate-sick-check):diamonds: - clausal proof checker (DRAT, DPR) for certifying SAT solvers' unsatisfiability results.
- [rlfsc](https://github.com/alex-ozdemir/rlfsc) [:package:](https://crates.io/crates/rlfsc) - checker for the LFSC proof language.
- [second_opinion](https://github.com/ammkrn/second_opinion) - verifier for Metamath Zero proof files.
- [smetamath](https://github.com/sorear/smetamath-rs) [:package:](https://crates.io/crates/smetamath) :star: - parallel and incremental verifier for Metamath databases.
- [t3p](https://github.com/skbaek/tesc/tree/master/t3p-rs) - optimized TESC (Theory-Extensible Sequent Calculus) verifier.
- [Verifier](https://github.com/trivial-rs/verifier) - Trivial proof verifier - an interface to the Metamath Zero kernel.

### Libraries

#### Parser

- [CNF Parser](https://github.com/robbepop/cnf-parser) [:package:](https://crates.io/crates/cnf-parser) - efficient and customizable parser for the .cnf file format.
- [DIMACS Parser](https://github.com/robbepop/dimacs-parser) [:package:](https://crates.io/crates/dimacs) - utilities to parse files in DIMACS .cnf or .sat file format.
- [Flussab CNF](https://github.com/jix/flussab) [:package:](https://crates.io/crates/flussab-cnf) - parsing and writing of the DIMACS CNF file format.
- [mmb-parser](https://github.com/trivial-rs/mmb-parser) [:package:](https://crates.io/crates/mmb-parser) - parser for the Metamath Zero binary proof format.
- [olean-rs](https://github.com/digama0/olean-rs) - parser/viewer for olean files.
- [smt2](https://github.com/regular-pv/smt2) [:package:](https://crates.io/crates/smt2) - SMT-LIB 2 parsing library.
- [tptp](https://github.com/MichaelRawson/tptp) [:package:](https://crates.io/crates/tptp):diamonds: - parse the TPTP format.

#### Bindings

- [CaDiCaL SAT solver](https://github.com/mmaroti/cadical-rs/) [:package:](https://crates.io/crates/cadical) - bindings for the CaDiCaL SAT solver.
- [libsmt.rs](https://github.com/sushant94/libsmt.rs) - bindings for SMTLIB2.
- [rsmt2](https://github.com/kino-mc/rsmt2) [:package:](https://crates.io/crates/rsmt2)[:package:](https://crates.io/crates/rsmt2-zz):star: - generic library to interact with SMT-LIB 2 compliant solvers.
- [Rust-SMT-LIB-API](https://github.com/facebookarchive/Rust-SMT-LIB-API)[:package:](https://crates.io/crates/rust_smt):skull::star: - generic high-level API for interacting with SMT solvers.
- [rustproof-libsmt](https://github.com/Rust-Proof/libsmt.rs) [:package:](https://crates.io/crates/rustproof-libsmt) - fork of libsmt.rs.

#### Translator

- [anthem](https://github.com/potassco/anthem) - translate answer set programs to first-order theorem prover language.
- [Cnfpack](https://github.com/jix/cnfpack) [:package:](https://crates.io/crates/cnfpack) - converts between the text based DIMACS CNF file format and the compressed binary Cnfpack format.
- [hz-to-mm0](https://github.com/digama0/hz-to-mm0) - translator from HOL Zero / Common HOL to Metamath Zero.

#### Misc

- [AbsoluteUnity](https://github.com/ray-kast/AbsoluteUnity) - think Prolog, but less capable.
- [compiler](https://github.com/trivial-rs/compiler) :baby_chick: - trivial compiler framework for Metamath Zero binary proofs.
- [discrimination-tree](https://github.com/MichaelRawson/discrimination-tree) [:package:](https://crates.io/crates/discrimination-tree) - discrimination tree term indexing.
- [egg](https://github.com/egraphs-good/egg) [:package:](https://crates.io/crates/egg):star: - flexible, high-performance e-graph library.
- [epilog](https://github.com/ray-kast/epilog) [:package:](https://crates.io/crates/epilog) - collection of Prolog-like tools for inference logic.
- [FALL](https://github.com/remexre/fall) [:package:](https://crates.io/crates/fall) - easily embeddable, futures-friendly logic engine.
- [Fathom](https://github.com/yeslogic/fathom) [:package:](https://crates.io/crates/fathom):star: - declarative data definition language for formally specifying binary data formats.
- [foliage](https://github.com/potassco/foliage) [:package:](https://crates.io/crates/foliage) - first-order logic with integer arithmetics.
- [Kravanenn](https://github.com/ppedrot/kravanenn) :star: - set of tools for Coq.
- [linear_solver](https://github.com/advancedresearch/linear_solver) [:package:](https://crates.io/crates/linear_solver):star: - linear solver designed to be easy to use with Rust enums.
- [mm0-rs](https://github.com/digama0/mm0/tree/master/mm0-rs) [:package:](https://crates.io/crates/mm0b_parser)[:package:](https://crates.io/crates/mm0_deepsize)[:package:](https://crates.io/crates/mm0_util):star: - MM0/MM1 server and utilities.
- [mmb-binutils](https://github.com/trivial-rs/mmb-binutils) - utility tools for Metamath Zero binary proof files.
- [mmb-types](https://crates.io/crates/mmb-types) - library containing the definitions of the opcodes in the Metamath Zero binary proof files.
- [moniker](https://github.com/brendanzab/moniker) [:package:](https://crates.io/crates/moniker)[:package:](https://crates.io/crates/moniker-derive):star: - automagical variable binding library. 
- [nanoda](https://github.com/ammkrn/nanoda) :skull::star: - became nanoda-lib.
- [nanoda_lib](https://github.com/ammkrn/nanoda_lib) - type inference/checking functionality based on the Lean theorem prover.
- [polytype](https://github.com/lucasem/polytype-rs) [:package:](https://crates.io/crates/polytype):star: - Hindley-Milner polymorphic typing system.
- [program-induction](https://github.com/lucasem/program-induction) [:package:](https://crates.io/crates/programinduction):star: - library for program induction and learning representations.
- [Prop](https://github.com/advancedresearch/prop) [:package:](https://crates.io/crates/prop) - library for theorem proving with Intuitionistic Propositional Logic.
- [rs-logik](https://github.com/SolarLiner/rs-logik) [:ghost:](https://github.com/newca12/rs-logik) - propositional logic interpreter.
- [rust-nbe-for-mltt](https://github.com/brendanzab/rust-nbe-for-mltt) :star: - normalization by evaluation for Martin-Löf Type Theory with dependent records.
- [rust-unify](https://github.com/bongo227/rust-unify) [:package:](https://crates.io/crates/rust-unify) :recycle: - unification algorithum implementation.
- [Rusty Razor](https://github.com/salmans/rusty-razor) [:package:](https://crates.io/crates/razor)[:package:](https://crates.io/crates/razor-fol)[:package:](https://crates.io/crates/razor-chase):star: - tool for constructing finite models for first-order theories.
- [smt2utils](https://github.com/facebookincubator/smt2utils) [:package:](https://crates.io/crates/smt2parser)[:package:](https://crates.io/crates/smt2patch)[:package:](https://crates.io/crates/smt2proxy)[:package:](https://crates.io/crates/z3tracer) - libraries and tools for the SMT-LIB-2 standard.
- [term-rewriting-rs](https://github.com/joshrule/term-rewriting-rs) [:package:](https://crates.io/crates/term_rewriting) :star: - library for representing, parsing, and computing with first-order term rewriting systems.
- [The Trivial Metamath Zero kernel](https://github.com/trivial-rs/kernel) [:package:](https://crates.io/crates/trivial-kernel) - Metamath Zero kernel for Trivial.
- [Whisper](https://github.com/sdleffler/whisper) :star: - logic Programming DSL.

## Books code

*There is [numerous](https://github.com/search?l=Rust&q=tapl&type=Repositories) implementations of TAPL [:book:](https://www.cis.upenn.edu/~bcpierce/tapl/), we keep only the most popular and keep an eye on implementations that worth attention.*

- [logic-rs](https://github.com/ixjf/logic-rs) [:book:](https://ruccs.rutgers.edu/lepore-meaning-and-argument/lepore-about-the-book):skull::star: - parser of relational predicate logic & truth tree solver
- [plar-rs](https://github.com/nikomatsakis/plar-rs) [:book:](https://www.cl.cam.ac.uk/~jrh13/atp/)[:ghost:](https://github.com/newca12/plar-rs) - exploring John Harrison's Handbook of Practical Logic and Automated Reasoning.
- [tapl](https://github.com/v4kst1z/tapl) - implementation of TAPL.
- [TAPL in Rust](https://github.com/hayatoito/tapl-in-rust) :star: - another collection of implementations of TAPL.
- [tnt](https://github.com/SymmetricChaos/tnt) [:book:](https://en.wikipedia.org/wiki/G%C3%B6del,_Escher,_Bach)[:package:](https://crates.io/crates/tnt) - implementation of Hofstader's "Typographical Number Theory" from the book Gödel, Escher, and Bach.
- [types-and-programming-languages](https://github.com/lazear/types-and-programming-languages) :star: - Exercises from Benjamin Pierce's "Types and Programming Languages" textbook + extras!

## Programming Language

- [egglog](https://github.com/philzook58/egglog) :star: - using the egg library with a file format and semantics similar to datalog.
- [Last Order Logic](https://github.com/advancedresearch/last_order_logic.git) [:package:](https://crates.io/crates/last_order_logic) - experimental logical language.
- [minitt-rs](https://github.com/owo-lang/minitt-rs) [:package:](https://crates.io/crates/minitt)[:package:](https://crates.io/crates/minitt-util/):skull::star: - became Voile.
- [Narc](https://github.com/owo-lang/narc-rs) [:package:](https://crates.io/crates/nar):star: - dependently-typed programming language with Agda style dependent pattern matching.
- [Pikelet](https://github.com/pikelet-lang/pikelet) [:package:](https://crates.io/crates/pikelet):star: - small, functional, dependently typed programming language.
- [proto-vulcan](https://github.com/terohuttunen/proto-vulcan) [:package:](https://crates.io/crates/proto-vulcan)[:package:](https://crates.io/crates/proto-vulcan-macros) - miniKanren-family relational logic programming language.
- [Scryer Prolog](https://github.com/mthom/scryer-prolog) [:package:](https://crates.io/crates/scryer-prolog):star: - modern Prolog implementation.
- [Symmetric Interaction Calculus](https://github.com/maiavictor/symmetric-interaction-calculus) :star: - programming language and model of computation that matches the optimal λ-calculus reduction algorithm perfectly.
- [Voile](https://github.com/owo-lang/voile-rs) [:package:](https://crates.io/crates/voile)[:package:](https://crates.io/crates/voile-util):skull::star: - became Narc.

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
- [Lamcal](https://github.com/haraldmaida/lamcal) [:package:](https://crates.io/crates/lamcal)[:package:](https://crates.io/crates/lamcal-repl) - lambda calculus parser and evaluator and a separate command line REPL.

### Unclassified

- [formal-systems-learning-rs](https://github.com/joshrule/formal-systems-learning-rs) - simulations using 2AFC triads to learn formal systems as typed first-order term rewriting systems.
- [list-routine-learning-rs](https://github.com/joshrule/list-routine-learning-rs) - simulations using input/output examples to learn typed first-order term rewriting systems that perform list routines.
- [n-queens-sat](https://github.com/erohkohl/n-queens-sat) - modelling n-queens problem as conjunctive normal form and solving it with DPLL algorithm.
- [nonogrid](https://github.com/tsionyx/nonogrid)[:package:](https://crates.io/crates/nonogrid) - lightning fast nonogram solver.
- [sudoku_sat](https://github.com/shnarazk/sudoku_sat) - solve Sudoku variants with SAT solvers.
- [Supermux](https://github.com/tuzz/supermux) - reduction of the superpermutation problem to Quantified Boolean Formula.
- [Supersat](https://github.com/tuzz/supersat) - attempt to find superpermutations by reducing the problem to SAT.
- [tarpit-rs](https://github.com/sdleffler/tarpit-rs) :star: - type-level implementation of Smallfuck in Rust, doubling as a Turing-completeness proof for Rust's type system.

## Resources

### Books

- [Verification for Dummies: SMT and Induction](https://ocamlpro.github.io/verification_for_dummies/) - broadly discusses induction as a formal verification technique.

### Thesis

- [Simple Verification of Rust Programs via Functional Purification](https://pp.ipd.kit.edu/uploads/publikationen/ullrich16masterarbeit.pdf) - thesis.
- [Understanding and Evolving the Rust Programming Language](https://www.ralfj.de/research/thesis.html) - first formal foundations for Rust: RustBelt and Stacked Borrows.

### Blogs

- [A Formal Verification of Rust's Binary Search Implementation](https://kha.github.io/) :uk:
- [Splr notebook.](https://shnarazk.github.io/tag/splr) :jp:
- [Research notebook about improving with Rust the performance of nonclausal automated theorem provers.](https://github.com/01mf02/adam-notes) :uk:
- [Varisat notebook.](https://jix.one/blog/rust/) :uk:

### Crates keywords

- [solver](https://crates.io/keywords/solver) - 61 entries.
- [logic](https://crates.io/keywords/logic) - 38 entries.
- [sat](https://crates.io/keywords/sat) - 25 entries.
- [smt](https://crates.io/keywords/smt) - 23 entries.
- [satisfiability](https://crates.io/keywords/satisfiability) - 23 entries.
- [verification](https://crates.io/keywords/verification) - 23 entries.
- [prover](https://crates.io/keywords/prover) - 7 entries.
- [rewriting](https://crates.io/keywords/rewriting) - 7 entries.
- [first-order](https://crates.io/keywords/first-order) - 6 entries.
- [cnf](https://crates.io/keywords/cnf) - 6 entries.
- [smt-lib](https://crates.io/keywords/smt-lib) - 6 entries.
- [metamath-zero](https://crates.io/keywords/metamath-zero) - 5 entries.
- [z3](https://crates.io/keywords/z3) - 5 entries.
- [dependent-types](https://crates.io/keywords/dependent-types) - 4 entries.
- [stark](https://crates.io/keywords/stark) - 4 entries.
- [dimacs](https://crates.io/keywords/dimacs) - 4 entries.

### Community

- [Johannes Altmanninger](https://github.com/krobelus) - rate.
- [ammkrn](https://twitter.com/ammkrn) - anoda, anoda_lib, second_opinion.
- [Mikko Aarnos](https://github.com/mAarnos) - Serkr.
- [Mathieu Baudet](https://github.com/matbd) - smt2utils.
- [Yechan Bae](https://qwaz.github.io/) - Rudra, Satire.
- [Clark Barrett](https://github.com/cbarrettfb) - Rust-SMT-LIB-API.
- [Remco Bloemen](https://2π.com) - OpenZKP Stark.
- [Mario Carneiro](https://www.cmu.edu/dietrich/philosophy/people/phd/mario-carneiro.html) - frat-rs, hz-to-mm0, mm0-rs, olean-rs, smetamath.
- [Adrien Champion](https://github.com/AdrienChampion) - hoice, Kinō, Mikino, rsmt2, SAT-MICRO, Verification for Dummies.
- [Simon Cruanes](https://simon.cedeela.fr/) - BatSat.
- [Xavier Denis](https://www.lri.fr/membre_en.php?mb=2819) - Creusot.
- [Sushant Dinesh](https://github.com/sushant94) - libsmt.rs.
- [Mark Drobnak](https://github.com/AzureMarker) - p4-analyzer.
- [Andrii Dmytrenko](https://uk.linkedin.com/in/andriidmytrenko) - lapjv.
- [Thomas Dziedzic](https://www.thomasdziedzic0.com/) - lambda_calculus.
- [Michael Färber](http://cl-informatik.uibk.ac.at/users/mfaerber) - CoP, Kontroli, meancop, research notebook about improving with Rust the performance of nonclausal automated theorem provers.
- [Robin Freyler](https://robbepop.github.io) - CNF Parser, DIMACS Parser.
- [Galois, Inc.](http://galois.com/) - crux-mir.
- [Nathan Graule ](https://github.com/SolarLiner) - rs-logik.
- [Masaki Hara](https://twitter.com/qnighy) - Logic solver, RatSat.
- [Jannis Harder](https://jix.one/) - Cnfpack, Flussab CNF, starlit, Varisat, Varisat notebook.
- [Timothée Haudebourg](https://github.com/timothee-haudebourg) - smt2.
- [Tero Huttunen](https://github.com/terohuttunen) - proto-vulcan.
- [Evan Johnson](https://github.com/enjhnsn2) - VeriWasm.
- [Ralf Jung](https://www.ralfj.de) - Understanding and Evolving the Rust Programming Language.
- [Irakliy Khaburzaniya](https://github.com/irakliyk) - Winterfell.
- [Prateek Kumar](https://prateekkumar.in) - msat, rsat, slp, SolHOP.
- [Ivan Ladelshchikov](https://github.com/tsionyx) - nonogrid.
- [ljedrz](https://github.com/ljedrz) - blc, lambda_calculus.
- [Shea Leffler](http://loud.fyi) - tarpit-rs, whisper. 
- [Patrick Lühne](https://www.luehne.de) - anthem, foliage.
- [mcmfb](https://github.com/mcmfb) - lambda_calc.
- [Victor Maia](https://medium.com/@maiavictor) - Symmetric Interaction Calculus.
- [Harald Maida](https://github.com/haraldmaida) - Lamcal.
- [Miklos Maroti](https://www.math.u-szeged.hu/~mmaroti) - cadical-rs, uasat-rs. 
- [Niko Matsakis](http://smallcultfollowing.com/babysteps) - Chalk, plar-rs.
- [Yusuke Matsushita](https://github.com/shiatsumat) - RustHorn.
- [Lucas Morales](https://lucasem.com) - polytype, program-induction.
- [Sven Nilsen](https://twitter.com/bvssvni) - Avalog, Debug-SAT, Last Order Logic, linear_solver, Monotonic-Solver, pocket_prover, pocket_prover-set, Poi, Prop, reachability_solver.
- [Yuichi Nishiwaki](http://hagi.is.s.u-tokyo.ac.jp/~yuichi/) - shari.
- [Alex Ozdemir](https://cs.stanford.edu/~aozdemir) - rlfsc.
- [Chris Patuzzo](https://tuzz.tech) - Supermux, Supersat.
- [Pierre-Marie Pédrot](https://www.pédrot.fr) - Kravanenn. 
- [Dan Pittman](https://dpitt.me) - Bounded Registers.
- [Christian Poveda](https://github.com/pvdrz) - Chevre.
- [Michael Rawson](http://rawsons.uk/michael) - discrimination-tree, lazyCoP, lerna, SATCoP, tptp.
- [Alastair Reid](https://alastairreid.github.io) - Rust verification tools list.
- [Nathan Ringo](https://remexre.xyz) - FALL.
- [Erik Rohkohl](https://blogs.itemis.com/author/erik-rohkohl) - n-queens-sat.
- [Josh Rule](http://www.joshrule.com) - formal-systems-learning-rs, list-routine-learning-rs, term-rewriting-rs. 
- [Salman Saghafi](https://github.com/salmans) - Rusty Razor.
- [Michael Salter](https://github.com/salterm) - Rustproof, rustproof-libsmt.
- [Ryan Schroeder](https://ryan-s.net/) - AbsoluteUnity, epilog.
- [Srinath Setty](https://www.microsoft.com/en-us/research/people/srinath) - Nova, Spartan.
- [skbaek](https://github.com/skbaek) - t3p.
- [Narazaki Shuji](https://shnarazk.github.io) - Splr, Splr notebook, sudoku_sat.
- [SymmetricChaos](https://github.com/SymmetricChaos) - tnt.
- [Mark Thom](https://github.com/mthom) - Scryer Prolog.
- [Hitoshi Togasaki](https://github.com/togatoga) - screwsat.
- [Sebastian Ullrich](https://twitter.com/derKha) - A Formal Verification of Rust's Binary Search Implementation, electrolysis, Simple Verification of Rust Programs via Functional Purification.
- [V4kst1z](https://github.com/v4kst1z) - tapl, TIP.
- [Max Willsey](https://www.mwillsey.com) - egg.
- [Ivo Wingelaar](https://github.com/IvoWingelaar) - compiler, mmb-binutils, mmb-parser, mmb-types, The Trivial Metamath Zero kernel, Verifier.
- [Jieyou Xu](https://github.com/jieyouxu) - Propositional Tableaux Solver.
- [Brendan Zabarauskas](https://github.com/brendanzab) - Fathom, moniker, Pikelet, rust-nbe-for-mltt.
- [Eric Zhang](https://www.ekzhang.com) - µKanren-rs.
- [Tesla Ice Zhang](https://ice1000.org) - minitt-rs, Narc, Voile.
- [Li Zhuohua](https://zhuohua.me/) - MirChecker.
- [Philip Zucker](http://www.philipzucker.com) - egglog.