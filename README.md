## About ##
A curated list of (sometimes) awesome Rust resources regarding automated or semi-automated formalization efforts in any area, including classical mathematics, constructive mathematics formal algorithms, and program verification.

awesome-rust-formalized-reasoning is an EDLA project.

The purpose of [edla.org](http://www.edla.org) is to promote the state of the art in various domains.


## Contents

- [Projects](#projects)
  - [Provers](#provers)
  - [Verification](#verification)
  - [Libraries](#libraries)
  - [Books](#books)
  - [Kanren](#kanren)
  - [Lambda_Calculus](lambda_calculus)
- [Resources](#resources)
  - [Thesis](#thesis)
  - [Community](#community)

---

## Legend

- Abandoned :skull:
- List of resources :information_source:
- No other alternatives :diamonds:

## Projects

### Provers

- [Avalog](https://crates.io/crates/avalog) - experimental implementation of Avatar Logic with a Prolog-like syntax.
- [Debug-SAT](https://crates.io/crates/debug_sat) - debuggable automatic theorem prover for boolean satisfiability problems (SAT).
- [CoP](https://crates.io/crates/cop) - reimplement in Rust several automated theorem provers of the leanCoP family, such as leanCoP and nanoCoP.
- [lazyCoP](https://github.com/MichaelRawson/lazycop) - automatic theorem prover for first-order logic with equality.
- [lapjv](https://crates.io/crates/lapjv) - linear Assignmment Problem solver using Jonker-Volgenant algorithm.
- [lerna](https://github.com/MichaelRawson/lerna) :skull: - proves theorems.
- [meancop](https://crates.io/crates/meancop) :skull: - became CoP.
- [Monotonic-Solver](https://crates.io/crates/monotonic_solver) - monotonic solver designed to be easy to use with Rust enum expressions.
- [OpenZKP Stark](https://crates.io/crates/zkp-stark) - implementation of STARK zero-knowledge-proofs.
- [pocket_prover](https://github.com/advancedresearch/pocket_prover) [:package:](https://crates.io/crates/pocket_prover)[:package:](https://crates.io/crates/pocket_prover-derive) - fast, brute force, automatic theorem prover for first order logic.
- [Poi](https://crates.io/crates/poi) - pragmatic point-free theorem prover assistant.
- [Resolution Prover](https://github.com/ExcaliburZero/resolution-prover) - resolution prover library for propositional logic.
- [SATCoP](https://github.com/MichaelRawson/satcop) - theorem prover for first-order logic based on connection tableau and SAT solving.
- [UASAT-RS](https://github.com/mmaroti/uasat-rs) - AT solver based calculator for discrete mathematics and universal algebra.

### Verification

- [Bounded Registers](https://crates.io/crates/bounded-registers) - high-assurance memory-mapped register interaction library.
- [CaDiCaL SAT solver](https://crates.io/crates/cadical) - bindings for the CaDiCaL SAT solver.
- [Chalk](https://github.com/rust-lang/chalk) - implements the Rust trait system, based on Prolog-ish logic rules.
- [Chevre](https://github.com/pvdrz/chevre) :skull: - small propositional logic interpreter.
- [Creusot](https://github.com/xldenis/creusot) - tool for deductive verification of Rust code.
- [crux-mir](https://github.com/GaloisInc/crucible/tree/master/crux-mir) - static simulator for Rust programs. It runs a set of test cases and attempts to prove that all assertions pass on all valid inputs.
- [kocheck](https://crates.io/crates/kocheck) :skull: -  became Kontroli.
- [Kontroli](https://crates.io/crates/kontroli) - alternative implementation of the logical framework Dedukti, concentrating on the verification of proofs.
- [pocket_prover-set](https://crates.io/crates/pocket_prover-set) - base logical system for PocketProver to reason about set properties.
- [Prusti](https://www.pm.inf.ethz.ch/research/prusti.html) - prototype verifier for Rust, built upon the the Viper verification infrastructure.
- [Rust verification tools list](https://alastairreid.github.io/rust-verification-tools/) :information_source: - list of tools
- [smetamath](https://crates.io/crates/smetamath) - parallel and incremental verifier for Metamath databases.
- [Scryer Prolog](https://crates.io/crates/scryer-prolog) - modern Prolog implementation.
- [Verifier](https://github.com/trivial-rs/verifier) - Trivial proof verifier - an interface to the Metamath Zero kernel.

### Libraries

- [anthem](https://github.com/potassco/anthem) - translate answer set programs to first-order theorem prover language.
- [Closure Calculus](https://crates.io/crates/closure_calculus) - library for Barry Jay's Closure Calculus.
- [compiler](https://github.com/trivial-rs/compiler) - Trivial compiler framework for Metamath Zero binary proofs.
- [discrimination-tree](https://crates.io/crates/discrimination-tree) - discrimination tree term indexing.
- [Fathom](https://crates.io/crates/fathom) - declarative data definition language for formally specifying binary data formats.
- [foliage](https://crates.io/crates/foliage) - First-order logic with integer arithmetics.
- [formal-systems-learning-rs](https://github.com/joshrule/formal-systems-learning-rs) - simulations using 2AFC triads to learn formal systems as typed first-order term rewriting systems.
- [Kravanenn](https://github.com/ppedrot/kravanenn) - set of tools for Coq.  
- [list-routine-learning-rs](https://github.com/joshrule/list-routine-learning-rs) - simulations using input/output examples to learn typed first-order term rewriting systems that perform list routines.
- [logic-rs](https://github.com/ixjf/logic-rs) :skull: - parser of relational predicate logic & truth tree solver.
- [minitt-rs](https://github.com/owo-lang/minitt-rs) [:package:](https://crates.io/crates/minitt)[:package:](https://crates.io/crates/minitt-util/) :skull: - became Voile.
- [mm0-rs](https://github.com/digama0/mm0/tree/master/mm0-rs) - MM0/MM1 server.
- [mmb-binutils](https://github.com/trivial-rs/mmb-binutils) - utility tools for Metamath Zero binary proof files.
- [mmb-parser](https://crates.io/crates/mmb-parser) - parser for the Metamath Zero binary proof format
- [mmb-types](https://crates.io/crates/mmb-types) - library containing the definitions of the opcodes in the Metamath Zero binary proof files.
- [moniker](https://github.com/brendanzab/moniker) [:package:](https://crates.io/crates/moniker)[:package:](https://crates.io/crates/moniker-derive) - automagical variable binding library. 
- [n-queens-sat](https://github.com/erohkohl/n-queens-sat) - Modelling n-queens problem as conjunctive normal form and solving it with DPLL algorithm.
- [nanoda](https://github.com/ammkrn/nanoda) :skull: - became nanoda-lib.
- [nanoda_lib](https://github.com/ammkrn/nanoda_lib) - type inference/checking functionality based on the Lean theorem prover.
- [Narc](https://crates.io/crates/nar) - dependently-typed programming language with Agda style dependent pattern matching.
- [olean-rs](https://github.com/digama0/olean-rs) - parser/viewer for olean files.
- [Pikelet](https://crates.io/crates/pikelet) - small, functional, dependently typed programming language.
- [polytype](https://crates.io/crates/polytype) - Hindley-Milner polymorphic typing system.
- [program-induction](https://crates.io/crates/programinduction) - library for program induction and learning representations.
- [rust-nbe-for-mltt](https://github.com/brendanzab/rust-nbe-for-mltt) - normalization by evaluation for Martin-Löf Type Theory with dependent records.
- [rust-unify](https://crates.io/crates/rust-unify) :skull: - unification algorithum implementation.
- [Rusty Razor](https://github.com/salmans/rusty-razor) [:package:](https://crates.io/crates/razor)[:package:](https://crates.io/crates/razor-fol)[:package:](https://crates.io/crates/razor-chase) - tool for constructing finite models for first-order theories.
- [Splr](https://crates.io/crates/splr) - modern CDCL SAT solver.
- [sudoku_sat](https://github.com/shnarazk/sudoku_sat) - solve Sudoku variants with SAT solvers.
- [Symmetric Interaction Calculus](https://github.com/maiavictor/symmetric-interaction-calculus) - programming language and model of computation that matches the optimal λ-calculus reduction algorithm perfectly.
- [tarpit-rs](https://github.com/sdleffler/tarpit-rs) - type-level implementation of Smallfuck in Rust, doubling as a Turing-completeness proof for Rust's type system.
- [term-rewriting-rs](https://crates.io/crates/term_rewriting) - library for representing, parsing, and computing with first-order term rewriting systems.
- [tptp](https://crates.io/crates/tptp) :diamonds: - parse the TPTP format.
- [The Trivial Metamath Zero kernel](https://crates.io/crates/trivial-kernel) - Metamath Zero kernel for Trivial.
- [Voile](https://github.com/owo-lang/voile-rs) [:package:](https://crates.io/crates/voile)[:package:](https://crates.io/crates/voile-util) :skull: - became Narc.
- [Whisper](https://github.com/sdleffler/whisper) - logic Programming DSL.

### Books

- [plar-rs](https://github.com/nikomatsakis/plar-rs) - Exploring John Harrison's Handbook of Practical Logic and Automated Reasoning.
- [TAPL in Rust](https://github.com/hayatoito/tapl-in-rust) - another collection of implementations of TAPL.
- [tapl-rust](https://github.com/ilya-klyuchnikov/tapl-rust)
- [types-and-programming-languages](https://github.com/lazear/types-and-programming-languages) - Exercises from Benjamin Pierce's "Types and Programming Languages" textbook + extras!

### Kanren

- [Canrun](https://crates.io/crates/canrun) - logic programming library inspired by the *Kanren family of language DSLs.
- [miniKANREN](https://crates.io/crates/mini-kanren) - miniKANREN as a DSL.
- [rslogic](https://crates.io/crates/rslogic) - logic programming framework for Rust inspired by µKanren.
- [rust-kanren](https://github.com/wartmanm/rust-kanren) - loose interpretation of miniKanren and cKanren.

### Lambda_Calculus

- [blc](https://crates.io/crates/blc) - implementation of the binary lambda calculus.
- [lambda_calc](https://crates.io/crates/lambda_calc) - command-line untyped lambda calculus interpreter.
- [lambda_calculus](https://crates.io/crates/lambda_calculus) - simple, zero-dependency implementation of pure lambda calculus in.


## Resources

### Thesis

- [A Formal Verification of Rust's Binary Search Implementation](https://kha.github.io/2016/07/22/formally-verifying-rusts-binary-search.html) - post about ongoing master’s thesis.
- [Simple Verification of RustPrograms via Functional Purification](https://pp.ipd.kit.edu/uploads/publikationen/ullrich16masterarbeit.pdf) - thesis.

### Community

- [ammkrn](https://twitter.com/ammkrn) - anoda, anoda_lib.
- [Remco Bloemen](https://2π.com) - OpenZKP Stark.
- [Mario Carneiro](https://www.cmu.edu/dietrich/philosophy/people/phd/mario-carneiro.html) - mm0-rs, olean-rs, smetamath.
- [Xavier Denis](https://www.lri.fr/membre_en.php?mb=2819) - Creusot.
- [Andrii Dmytrenko](https://uk.linkedin.com/in/andriidmytrenko) - lapjv.
- [Michael Färber](http://cl-informatik.uibk.ac.at/users/mfaerber) - CoP, kocheck, Kontroli, meancop.
- [Galois, Inc.](http://galois.com/) - crux-mir.
- [ljedrz](https://github.com/ljedrz) - blc, lambda_calculus.
- [Shea Leffler](http://loud.fyi) - tarpit-rs, whisper. 
- [Patrick Lühne](https://www.luehne.de) - anthem, foliage.
- [mcmfb](https://github.com/mcmfb) - lambda_calc.
- [Victor Maia](https://medium.com/@maiavictor) - Symmetric Interaction Calculus.
- [Miklos Maroti](https://www.math.u-szeged.hu/~mmaroti) - cadical-rs, uasat-rs. 
- [Niko Matsakis](http://smallcultfollowing.com/babysteps) - Chalk, plar-rs
- [Lucas Morales](https://lucasem.com) - polytype, program-induction.
- [Sven Nilsen](https://twitter.com/bvssvni) - Avalog, Debug-SAT, Monotonic-Solver, pocket_prover, pocket_prover-set, Poi.
- [Pierre-Marie Pédrot](https://www.pédrot.fr) - Kravanenn. 
- [Dan Pittman](https://dpitt.me) - Bounded Registers.
- [Christian Poveda](https://github.com/pvdrz) - Chevre.
- [Michael Rawson](http://rawsons.uk/michael) - discrimination-tree, lazyCoP, lerna, SATCoP, tptp.
- [Alastair Reid](https://alastairreid.github.io) - Rust verification tools list.
- [Erik Rohkohl](https://blogs.itemis.com/author/erik-rohkohl) - n-queens-sat.
- [Josh Rule](http://www.joshrule.com) - formal-systems-learning-rs, list-routine-learning-rs, term-rewriting-rs. 
- [Salman Saghafi](https://github.com/salmans) - Rusty Razor.
- [Narazaki Shuji](https://shnarazk.github.io) - Splr, sudoku_sat.
- [Mark Thom](https://github.com/mthom) - Scryer Prolog.
- [Sebastian Ullrich](https://twitter.com/derKha) - A Formal Verification of Rust's Binary Search Implementation, Simple Verification of RustPrograms via Functional Purification.
- [Ivo Wingelaar](https://github.com/IvoWingelaar) - compiler, mmb-binutils, mmb-parser, mmb-types, The Trivial Metamath Zero kernel, Verifier.
- [Brendan Zabarauskas]() - Fathom, moniker, Pikelet, rust-nbe-for-mltt. 
- [Tesla Ice Zhang](https://ice1000.org) - minitt-rs, Narc, Voile.