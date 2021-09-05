## About ##
An exhaustive list of all Rust resources regarding automated or semi-automated formalization efforts in any area, constructive mathematics, formal algorithms, and program verification.

awesome-rust-formalized-reasoning is an EDLA project.

The purpose of [edla.org](http://www.edla.org) is to promote the state of the art in various domains.


## Contents

- [Projects](#projects)
  - [Provers & Solvers](#provers-and-solvers)
  - [Verification](#verification)
  - [Libraries](#libraries)
  - [Books](#books)
  - [Kanren](#kanren)
  - [Lambda_Calculus](lambda_calculus)
- [Resources](#resources)
  - [Crates keywords](#crates-keywords)
  - [Thesis](#thesis)
  - [Blogs](#blogs)
  - [Community](#community)

---

## Legend

- Abandoned :skull:
- Toy project :baby_chick:
- List of resources :information_source:
- More than one crate :package:
- Best in Class :diamonds:
- Popular :star:
- Exhumated :ghost:
- Deleted :recycle:

## Projects

### Provers and Solvers

- [Avalog](https://crates.io/crates/avalog) :star: - experimental implementation of Avatar Logic with a Prolog-like syntax.
- [Debug-SAT](https://crates.io/crates/debug_sat) - debuggable automatic theorem prover for boolean satisfiability problems (SAT).
- [CoP](https://crates.io/crates/cop) - reimplement in Rust several automated theorem provers of the leanCoP family, such as leanCoP and nanoCoP.
- [egglog](https://github.com/philzook58/egglog) - Using the egg library with a file format and semantics similar to datalog.
- [lazyCoP](https://github.com/MichaelRawson/lazycop) - automatic theorem prover for first-order logic with equality.
- [lapjv](https://crates.io/crates/lapjv) - linear Assignmment Problem solver using Jonker-Volgenant algorithm.
- [lerna](https://github.com/MichaelRawson/lerna) :skull: - proves theorems.
- [Logic solver](https://github.com/qnighy/logic-solver-rs) :star: - Logic solver.
- [meancop](https://crates.io/crates/meancop) :skull: - became CoP.
- [Mikino](https://github.com/OCamlPro/mikino)[:package:](https://crates.io/crates/mikino)[:package:](https://crates.io/crates/mikino_api) - a simple induction and BMC engine.
- [Monotonic-Solver](https://crates.io/crates/monotonic_solver) :star: - monotonic solver designed to be easy to use with Rust enum expressions.
- [msat](https://crates.io/crates/msat) - MaxSAT Solver.
- [OpenZKP Stark](https://crates.io/crates/zkp-stark) :star: - implementation of STARK zero-knowledge-proofs.
- [pocket_prover](https://github.com/advancedresearch/pocket_prover) [:package:](https://crates.io/crates/pocket_prover)[:package:](https://crates.io/crates/pocket_prover-derive) :star: - fast, brute force, automatic theorem prover for first order logic.
- [Poi](https://crates.io/crates/poi) :star: - pragmatic point-free theorem prover assistant.
- [RatSat](https://github.com/qnighy/ratsat) [:package:](https://crates.io/crates/ratsat)[:package:](https://crates.io/crates/ratsat-bin) :star: - reimplementation of MiniSat.
- [reachability_solver](https://crates.io/crates/reachability_solver) - linear reachability solver for directional edges.
- [Resolution Prover](https://github.com/ExcaliburZero/resolution-prover) - resolution prover library for propositional logic.
- [rsat](https://crates.io/crates/rsat) - SAT Solver.
- [SATCoP](https://github.com/MichaelRawson/satcop) - theorem prover for first-order logic based on connection tableau and SAT solving.
- [SAT-MICRO](https://github.com/OCamlPro/sat_micro_rust) - a reimplementation of the SAT-solver described in SAT-MICRO: petit mais costaud! by Sylvain Conchon et al.
- [screwsat](https://crates.io/crates/screwsat) :star: - a simple CDCL SAT Solver.
- [Serkr](https://github.com/mAarnos/Serkr) [:ghost:](https://github.com/newca12/Serkr) :star: - automated theorem prover for first order logic with equality.
- [slp](https://crates.io/crates/slp) :skull: - became SolHOP.
- [SolHOP](https://crates.io/crates/solhop) - aims to be a SAT and MaxSAT solver. Currently, a CDCL based SAT.
- [UASAT-RS](https://github.com/mmaroti/uasat-rs) - SAT solver based calculator for discrete mathematics and universal algebra.
- [Varisat](https://github.com/jix/varisat)[:package:](https://crates.io/crates/varisat)[:package:](https://crates.io/crates/varisat-checker)[:package:](https://crates.io/crates/varisat-cli)[:package:](https://crates.io/crates/varisat-dimacs)[:package:](https://crates.io/crates/varisat-formula)[:package:](https://crates.io/crates/varisat-internal-macros)[:package:](https://crates.io/crates/varisat-internal-proof)[:package:](https://crates.io/crates/varisat-lrat) :star: - CDCL based SAT solver.
- [Winterfell](https://github.com/novifinancial/winterfell)[:package:](https://crates.io/crates/winter-air)[:package:](https://crates.io/crates/winter-crypto)[:package:](https://crates.io/crates/winterfell)[:package:](https://crates.io/crates/winter-fri)[:package:](https://crates.io/crates/winter-math)[:package:](https://crates.io/crates/winter-prover)[:package:](https://crates.io/crates/winter-utils)[:package:](https://crates.io/crates/winter-verifier) :star: - A STARK prover and verifier for arbitrary computations.

### Verification

- [Bounded Registers](https://crates.io/crates/bounded-registers) :star: - high-assurance memory-mapped register interaction library.
- [CaDiCaL SAT solver](https://crates.io/crates/cadical) - bindings for the CaDiCaL SAT solver.
- [Chalk](https://github.com/rust-lang/chalk) :star: - implements the Rust trait system, based on Prolog-ish logic rules.
- [Chevre](https://github.com/pvdrz/chevre) :recycle: - small propositional logic interpreter.
- [Creusot](https://github.com/xldenis/creusot) :star: - tool for deductive verification of Rust code.
- [crux-mir](https://github.com/GaloisInc/crucible/tree/master/crux-mir) :star: - static simulator for Rust programs. It runs a set of test cases and attempts to prove that all assertions pass on all valid inputs.
- [frat-rs](https://github.com/digama0/frat) - verify DIMACS proof.
- [Kontroli](https://github.com/01mf02/kontroli-rs)  [:package:](https://crates.io/crates/dedukti-parse)[:package:](https://crates.io/crates/kocheck)[:package:](https://crates.io/crates/kontroli) - alternative implementation of the logical framework Dedukti, concentrating on the verification of proofs.
- [p4-analyzer](https://github.com/AzureMarker/p4-analyzer) - static analysis tool which checks P4 code for bugs.
- [pocket_prover-set](https://crates.io/crates/pocket_prover-set) - base logical system for PocketProver to reason about set properties.
- [Prusti](https://www.pm.inf.ethz.ch/research/prusti.html) :star: - prototype verifier for Rust, built upon the the Viper verification infrastructure.
- [rate](https://github.com/krobelus/rate) [:package:](https://crates.io/crates/rate)[:package:](https://crates.io/crates/rate-common)[:package:](https://github.com/krobelus/rate)[:package:](https://crates.io/crates/rate-proof-utils)[:package:](https://crates.io/crates/rate-sick-check) :diamonds: - clausal proof checker (DRAT, DPR) for certifying SAT solvers' unsatisfiability results.
- [rlfsc](https://crates.io/crates/rlfsc) - A checker for the LFSC proof language.
- [Rust verification tools list](https://alastairreid.github.io/automatic-rust-verification-tools-2021/) :information_source: - list of tools
- [smetamath](https://crates.io/crates/smetamath) :star: - parallel and incremental verifier for Metamath databases.
- [Scryer Prolog](https://crates.io/crates/scryer-prolog) :star: - modern Prolog implementation.
- [t3p](https://github.com/skbaek/tesc/tree/master/t3p-rs) - optimized TESC (Theory-Extensible Sequent Calculus) verifier.
- [Verifier](https://github.com/trivial-rs/verifier) - Trivial proof verifier - an interface to the Metamath Zero kernel.

### Libraries

- [anthem](https://github.com/potassco/anthem) - translate answer set programs to first-order theorem prover language.
- [Closure Calculus](https://crates.io/crates/closure_calculus) - library for Barry Jay's Closure Calculus.
- [Cnfpack](https://crates.io/crates/cnfpack) - converts between the text based DIMACS CNF file format and the compressed binary Cnfpack format.
- [CNF Parser](https://crates.io/crates/cnf-parser) - efficient and customizable parser for the .cnf file format.
- [compiler](https://github.com/trivial-rs/compiler) - trivial compiler framework for Metamath Zero binary proofs.
- [DIMACS Parser](https://crates.io/crates/dimacs) - utilities to parse files in DIMACS .cnf or .sat file format.
- [discrimination-tree](https://crates.io/crates/discrimination-tree) - discrimination tree term indexing.
- [egg](https://crates.io/crates/egg) :star: - flexible, high-performance e-graph library.
- [Fathom](https://crates.io/crates/fathom) :star: - declarative data definition language for formally specifying binary data formats.
- [Flussab CNF](https://crates.io/crates/flussab-cnf) - parsing and writing of the DIMACS CNF file format
- [foliage](https://crates.io/crates/foliage) - first-order logic with integer arithmetics.
- [formal-systems-learning-rs](https://github.com/joshrule/formal-systems-learning-rs) - simulations using 2AFC triads to learn formal systems as typed first-order term rewriting systems.
- [hz-to-mm0](https://github.com/digama0/hz-to-mm0) - translator from HOL Zero / Common HOL to Metamath Zero.
- [Kravanenn](https://github.com/ppedrot/kravanenn) :star: - set of tools for Coq.
- [linear_solver](https://crates.io/crates/linear_solver) - linear solver designed to be easy to use with Rust enums.
- [list-routine-learning-rs](https://github.com/joshrule/list-routine-learning-rs) - simulations using input/output examples to learn typed first-order term rewriting systems that perform list routines.
- [logic-rs](https://github.com/ixjf/logic-rs) :skull: :star: - parser of relational predicate logic & truth tree solver.
- [minitt-rs](https://github.com/owo-lang/minitt-rs) [:package:](https://crates.io/crates/minitt)[:package:](https://crates.io/crates/minitt-util/) :skull: :star: - became Voile.
- [mm0-rs](https://github.com/digama0/mm0/tree/master/mm0-rs) [:package:](https://crates.io/crates/mm0b_parser)[:package:](https://crates.io/crates/mm0_deepsize)[:package:](https://crates.io/crates/mm0_util) :star: - MM0/MM1 server and utilities.
- [mmb-binutils](https://github.com/trivial-rs/mmb-binutils) - utility tools for Metamath Zero binary proof files.
- [mmb-parser](https://crates.io/crates/mmb-parser) - parser for the Metamath Zero binary proof format
- [mmb-types](https://crates.io/crates/mmb-types) - library containing the definitions of the opcodes in the Metamath Zero binary proof files.
- [moniker](https://github.com/brendanzab/moniker) [:package:](https://crates.io/crates/moniker)[:package:](https://crates.io/crates/moniker-derive) :star: - automagical variable binding library. 
- [n-queens-sat](https://github.com/erohkohl/n-queens-sat) - Modelling n-queens problem as conjunctive normal form and solving it with DPLL algorithm.
- [nanoda](https://github.com/ammkrn/nanoda) :skull: :star: - became nanoda-lib.
- [nanoda_lib](https://github.com/ammkrn/nanoda_lib) - type inference/checking functionality based on the Lean theorem prover.
- [Narc](https://crates.io/crates/nar) :star: - dependently-typed programming language with Agda style dependent pattern matching.
- [olean-rs](https://github.com/digama0/olean-rs) - parser/viewer for olean files.
- [Pikelet](https://crates.io/crates/pikelet) :star: - small, functional, dependently typed programming language.
- [polytype](https://crates.io/crates/polytype) :star: - Hindley-Milner polymorphic typing system.
- [program-induction](https://crates.io/crates/programinduction) :star: - library for program induction and learning representations.
- [Prop](https://crates.io/crates/prop) - library for theorem proving with Intuitionistic Propositional Logic.
- [rust-nbe-for-mltt](https://github.com/brendanzab/rust-nbe-for-mltt) :star: - normalization by evaluation for Martin-Löf Type Theory with dependent records.
- [rust-unify](https://crates.io/crates/rust-unify) :recycle: - unification algorithum implementation.
- [Rusty Razor](https://github.com/salmans/rusty-razor) [:package:](https://crates.io/crates/razor)[:package:](https://crates.io/crates/razor-fol)[:package:](https://crates.io/crates/razor-chase) :star: - tool for constructing finite models for first-order theories.
- [Splr](https://crates.io/crates/splr) :star: - modern CDCL SAT solver.
- [sudoku_sat](https://github.com/shnarazk/sudoku_sat) - solve Sudoku variants with SAT solvers.
- [Symmetric Interaction Calculus](https://github.com/maiavictor/symmetric-interaction-calculus) :star: - programming language and model of computation that matches the optimal λ-calculus reduction algorithm perfectly.
- [tarpit-rs](https://github.com/sdleffler/tarpit-rs) :star: - type-level implementation of Smallfuck in Rust, doubling as a Turing-completeness proof for Rust's type system.
- [term-rewriting-rs](https://crates.io/crates/term_rewriting) :star: - library for representing, parsing, and computing with first-order term rewriting systems.
- [tptp](https://crates.io/crates/tptp) :diamonds: - parse the TPTP format.
- [The Trivial Metamath Zero kernel](https://crates.io/crates/trivial-kernel) - Metamath Zero kernel for Trivial.
- [Voile](https://github.com/owo-lang/voile-rs) [:package:](https://crates.io/crates/voile)[:package:](https://crates.io/crates/voile-util) :skull: :star: - became Narc.
- [Whisper](https://github.com/sdleffler/whisper) :star: - logic Programming DSL.

### Books

- [plar-rs](https://github.com/nikomatsakis/plar-rs) [:ghost:](https://github.com/newca12/plar-rs) - Exploring John Harrison's Handbook of Practical Logic and Automated Reasoning.
- [TAPL in Rust](https://github.com/hayatoito/tapl-in-rust) :star: - another collection of implementations of TAPL.
- [tapl-rust](https://github.com/ilya-klyuchnikov/tapl-rust) :baby_chick: - very limited TAPL implemention.
- [tnt](https://crates.io/crates/tnt) - implementation of Hofstader's "Typographical Number Theory" from the book Gödel, Escher, and Bach.
- [types-and-programming-languages](https://github.com/lazear/types-and-programming-languages) :star: - Exercises from Benjamin Pierce's "Types and Programming Languages" textbook + extras!

### Kanren

- [Canrun](https://crates.io/crates/canrun) :star: - logic programming library inspired by the *Kanren family of language DSLs.
- [miniKANREN](https://crates.io/crates/mini-kanren) - miniKANREN as a DSL.
- [rslogic](https://crates.io/crates/rslogic) :star: - logic programming framework for Rust inspired by µKanren.
- [rust-kanren](https://github.com/wartmanm/rust-kanren) :star: - loose interpretation of miniKanren and cKanren.

### Lambda_Calculus

- [blc](https://crates.io/crates/blc) - implementation of the binary lambda calculus.
- [lambda_calc](https://crates.io/crates/lambda_calc) - command-line untyped lambda calculus interpreter.
- [lambda_calculus](https://crates.io/crates/lambda_calculus) :star: - simple, zero-dependency implementation of pure lambda calculus in safe Rust.
- [Lamcal](https://github.com/haraldmaida/lamcal) [:package:](https://crates.io/crates/lamcal)[:package:](https://crates.io/crates/lamcal-repl) - Lambda Calculus parser and evaluator and a separate command line REPL.


## Resources

### Thesis

- [A Formal Verification of Rust's Binary Search Implementation](https://kha.github.io/2016/07/22/formally-verifying-rusts-binary-search.html) - post about ongoing master’s thesis.
- [Simple Verification of Rust Programs via Functional Purification](https://pp.ipd.kit.edu/uploads/publikationen/ullrich16masterarbeit.pdf) - thesis.

### Blogs

- [Research notebook by Michael Färber about improving with Rust the performance of nonclausal automated theorem provers.](https://github.com/01mf02/adam-notes)

### Crates keywords

- [solver](https://crates.io/keywords/solver) - 61 entries.
- [logic](https://crates.io/keywords/logic) - 35 entries.
- [sat](https://crates.io/keywords/sat) - 25 entries.
- [smt](https://crates.io/keywords/smt) - 23 entries.
- [satisfiability](https://crates.io/keywords/satisfiability) - 23 entries.
- [verification](https://crates.io/keywords/verification) - 22 entries.
- [prover](https://crates.io/keywords/prover) - 7 entries.
- [rewriting](https://crates.io/keywords/rewriting) - 7 entries.
- [first-order](https://crates.io/keywords/first-order) - 6 entries.
- [cnf](https://crates.io/keywords/cnf) - 6 entries.
- [metamath-zero](https://crates.io/keywords/metamath-zero) - 5 entries.
- [dependent-types](https://crates.io/keywords/dependent-types) - 4 entries.
- [stark](https://crates.io/keywords/stark) - 4 entries.
- [dimacs](https://crates.io/keywords/dimacs) - 4 entries.

### Community

- [Johannes Altmanninger](https://github.com/krobelus) - rate.
- [ammkrn](https://twitter.com/ammkrn) - anoda, anoda_lib.
- [Mikko Aarnos](https://github.com/mAarnos) - Serkr.
- [Remco Bloemen](https://2π.com) - OpenZKP Stark.
- [Mario Carneiro](https://www.cmu.edu/dietrich/philosophy/people/phd/mario-carneiro.html) - frat-rs, hz-to-mm0, mm0-rs, olean-rs, smetamath.
- [Adrien Champion](https://github.com/AdrienChampion) - Mikino, SAT-MICRO.
- [Xavier Denis](https://www.lri.fr/membre_en.php?mb=2819) - Creusot.
- [Mark Drobnak](https://github.com/AzureMarker) - p4-analyzer.
- [Andrii Dmytrenko](https://uk.linkedin.com/in/andriidmytrenko) - lapjv.
- [Michael Färber](http://cl-informatik.uibk.ac.at/users/mfaerber) - CoP, Kontroli, meancop, research notebook by Michael Färber about improving with Rust the performance of nonclausal automated theorem provers.
- [Robin Freyler](https://robbepop.github.io/) - CNF Parser, DIMACS Parser.
- [Galois, Inc.](http://galois.com/) - crux-mir.
- [Masaki Hara](https://twitter.com/qnighy/) - Logic solver, RatSat.
- [Jannis Harder](https://jix.one/) - Cnfpack, Flussab CNF, Varisat.
- [Irakliy Khaburzaniya](https://github.com/irakliyk) - Winterfell.
- [Ilya Klyuchnikov](https://pat.keldysh.ru/~ilya/) - tapl-rust.
- [Prateek Kumar](https://prateekkumar.in/) - msat, rsat, slp, SolHOP.
- [ljedrz](https://github.com/ljedrz) - blc, lambda_calculus.
- [Shea Leffler](http://loud.fyi) - tarpit-rs, whisper. 
- [Patrick Lühne](https://www.luehne.de) - anthem, foliage.
- [mcmfb](https://github.com/mcmfb) - lambda_calc.
- [Victor Maia](https://medium.com/@maiavictor) - Symmetric Interaction Calculus.
- [Miklos Maroti](https://www.math.u-szeged.hu/~mmaroti) - cadical-rs, uasat-rs. 
- [Niko Matsakis](http://smallcultfollowing.com/babysteps) - Chalk, plar-rs
- [Harald Maida](https://github.com/haraldmaida) - Lamcal
- [Lucas Morales](https://lucasem.com) - polytype, program-induction.
- [Sven Nilsen](https://twitter.com/bvssvni) - Avalog, Debug-SAT, linear_solver, Monotonic-Solver, pocket_prover, pocket_prover-set, Poi, Prop, reachability_solver.
- [Alex Ozdemir](https://cs.stanford.edu/~aozdemir) - rlfsc.
- [Pierre-Marie Pédrot](https://www.pédrot.fr) - Kravanenn. 
- [Dan Pittman](https://dpitt.me) - Bounded Registers.
- [Christian Poveda](https://github.com/pvdrz) - Chevre.
- [Michael Rawson](http://rawsons.uk/michael) - discrimination-tree, lazyCoP, lerna, SATCoP, tptp.
- [Alastair Reid](https://alastairreid.github.io) - Rust verification tools list.
- [Erik Rohkohl](https://blogs.itemis.com/author/erik-rohkohl) - n-queens-sat.
- [Josh Rule](http://www.joshrule.com) - formal-systems-learning-rs, list-routine-learning-rs, term-rewriting-rs. 
- [Salman Saghafi](https://github.com/salmans) - Rusty Razor.
- [skbaek](https://github.com/skbaek) - t3p.
- [Narazaki Shuji](https://shnarazk.github.io) - Splr, sudoku_sat.
- [SymmetricChaos](https://github.com/SymmetricChaos) - tnt.
- [Mark Thom](https://github.com/mthom) - Scryer Prolog.
- [Hitoshi Togasaki](https://github.com/togatoga) - screwsat.
- [Sebastian Ullrich](https://twitter.com/derKha) - A Formal Verification of Rust's Binary Search Implementation, Simple Verification of Rust Programs via Functional Purification.
- [Max Willsey](https://www.mwillsey.com/) - egg.
- [Ivo Wingelaar](https://github.com/IvoWingelaar) - compiler, mmb-binutils, mmb-parser, mmb-types, The Trivial Metamath Zero kernel, Verifier.
- [Brendan Zabarauskas](https://github.com/brendanzab) - Fathom, moniker, Pikelet, rust-nbe-for-mltt.
- [Tesla Ice Zhang](https://ice1000.org) - minitt-rs, Narc, Voile.
- [Philip Zucker](http://www.philipzucker.com/) - egglog.