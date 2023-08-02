
FroCoS 2023 Accepted Papers with Abstracts
==========================================

Nils Lommen and [Jürgen Giesl](https://verify.rwth-aachen.de/giesl/).
**Targeting Completeness: Using Closed Forms for Size Bounds of Integer Programs**

**Abstract:** We present a new procedure to infer size bounds for integer programs automatically. Size bounds are important for the deduction of bounds on the runtime complexity or in general, for the resource analysis of programs. We show that our technique is complete (i.e., it always computes finite size bounds) for a subclass of loops, possibly with non-linear arithmetic. Moreover, we present a novel approach to combine and integrate this complete technique into an incomplete approach to infer size and runtime bounds of general integer programs. We prove completeness of our integration for an important subclass of integer programs. We implemented our new algorithm in the automated complexity analysis tool KoAT to evaluate its power, in particular on programs with non-linear arithmetic.

---

Visa Nummelin, [Jasmin Blanchette](https://www.tcs.ifi.lmu.de/mitarbeiter/jasmin-blanchette_de.html) and Sander R. Dahmen
**Recurrence-Driven Summations in Automated Deduction**

**Abstract:** Many problems in mathematics and computer science involve summations. We present a procedure that automatically proves equations involving finite summations, inspired by the theory of holonomic sequences. The procedure is designed to be interleaved with the activities of a higher-order automatic theorem prover. It performs an induction and automatically solves the induction step, leaving the base cases to the theorem prover.

---

Teppei Saito and [Nao Hirokawa](http://www.jaist.ac.jp/~hirokawa/)

**Weighted Path Orders are Semantic Path Orders**

**Abstract:** We explore the relationship between weighted path orders and (monotonic) semantic path orders. Our findings reveal that weighted path orders can be considered instances of a variant of semantic path orders that comprise order pairs. This observation leads to a generalization of weighted path orders that does not impose simplicity on underlying algebras. As a result, the generalized version is capable of proving termination of term rewrite systems beyond the realm of simple termination. In order to assess practicality we provide experimental data comparing generalized weighted path orders with original ones as well as other well-known classes of reduction orders.

---

Giorgio Cignarale, [Roman Kuznets](https://informatics.tuwien.ac.at/people/roman-kuznets), Hugo Rincon Galeana and Ulrich Schmid

**Logic of Communication Interpretation: How to not get lost in translation**

**Abstract:** Byzantine fault-tolerant distributed systems are designed to provide resiliency despite arbitrary faults, i.e., even in the presence of agents who do not follow the common protocol and/or despite compromised communication. It is, therefore, common to focus on the perspective of correct agents, to the point that the epistemic state of byzantine agents is completely ignored. Since this view relies on the assumption that faulty agents may behave arbitrarily adversarially, it is overly conservative in many cases. In blockchain settings, for example, dishonest players are usually not malicious, but rather selfish, and thus just follow some "hidden" protocol that is different from the protocol of the honest players. Similarly, in high-availability large-scale distributed systems, software updates cannot be globally instantaneous, but are rather performed node-by-node. Consequently, updated and non updated nodes may simultaneously be involved in a protocol for solving a distributed task like consensus or transaction commit. Clearly, the usual assumption of common knowledge of the protocol is inappropriate in such a setting. On the other hand, joint protocol execution and, sometimes, even basic communication becomes problematic without this assumption: How are agents supposed to interpret each other's messages without knowing their mutual communication protocols? We propose a novel epistemic modality \emph{creed} for epistemic reasoning in heterogeneous distributed systems with agents that are uncertain of the actual communication protocol used by their peers. We show that the resulting logic is quite closely related to modal logic S5, the standard logic of epistemic reasoning in distributed systems. We demonstrate the utility of our approach by several examples.

---

Guilherme Toledo, [Yoni Zohar](https://u.cs.biu.ac.il/~zoharyo1/) and Clark Barrett

**Combining Finite Combination Properties: Finite Models and Busy Beavers**

**Abstract:** This work is a part of an ongoing effort to understand the relationships between properties used in theory combination. We here focus on including two properties that are related to shiny theories: the finite model property and stable finiteness. For any combination of properties, we consider the question of whether there exists a theory that exhibits it. When there is, we provide an example with the simplest possible signature. One particular class of interest includes theories with the finite model property that are not finitely witnessable. To construct such theories, we utilize the Busy Beaver function.

---

Yasmine Briefs, [Christoph Weidenbach](https://www.mpi-inf.mpg.de/departments/automation-of-logic/people/christoph-weidenbach) and Hendrik Leidinger

**KBO Constraint Solving Revisited**

**Abstract:** KBO constraint solving is very well-known to be an NP-complete problem.
Motivated by the needs of the family of SCL calculi, we consider the particular
case where all terms occurring in a constraint are bound by a (single) ground term.
We show that this problem and variants of this problem remain NP-complete even if the form of atoms in the constraint
is further restricted. In addition, for a non-strict, partial term ordering solely based on symbol counting constraint solving remains NP-complete.
Nevertheless, we provide a new simple algorithm testing KBO constraint solvability that performs well on benchmark examples.

---

Burak Ekici, [Arjun Viswanathan](https://homepage.divms.uiowa.edu/~viswanathn/), Yoni Zohar, Cesare Tinelli and Clark Barrett

**Formal Verification of Bit-vector Invertibility Conditions in Coq**

**Abstract:** We prove the correctness of invertibility conditions for the theory
of fixed-width bit-vectors---used to solve quantified bit-vector formulas
in the Satisfiability Modulo Theories (SMT) solver cvc5--- in
the coq proof assistant. While many of these were proved in a completely
automatic fashion for arbitrary bit-width, some were only proved for bit-widths up
to 65, even though they are being used to solve formulas over larger
bit-widths. In this paper we describe the process of proving a
representative subset of these invertibility conditions in coq.
In particular, we describe the BVLIST library for bit-vectors
in coq, our extensions to it, and proofs of the invertibility conditions.

---

Olle Torstensson and [Tjark Weber](https://user.it.uu.se/~tjawe125/)

**Hammering Floating-Point Arithmetic**

**Abstract:** Sledgehammer, a component of the interactive proof assistant Isabelle/HOL, aims to increase proof automation by automatically discharging proof goals with the help of external provers. Among these provers are a group of satisfiability modulo theories (SMT) solvers with support for the SMT-LIB input language. Despite existing formalizations of IEEE floating-point arithmetic in both Isabelle/HOL and SMT-LIB, Sledgehammer employs an abstract translation of floating-point types and constants, depriving the SMT solvers of the opportunity to make use of their dedicated decision procedures for floating-point arithmetic.

We show that, by extending Sledgehammer's translation from the language of Isabelle/HOL into SMT-LIB with an interpretation of floating-point types and constants, floating-point reasoning in SMT solvers can be made available to Isabelle/HOL. Our main contribution is a description and implementation of such an extension. An evaluation of the extended translation shows a significant increase of Sledgehammer's success rate on proof goals involving floating-point arithmetic.

---

Liao Zhang, Lasse Blaauwbroek, [Cezary Kaliszyk](http://cl-informatik.uibk.ac.at/cek/) and Josef Urban

**Learning Proof Transformations and Its Applications in Interactive Theorem Proving**

**Abstract:** Interactive theorem provers are today increasingly used to certify mathematical theories. To formally prove a theorem, reasoning procedures called tactics are invoked successively on the proof states starting with the initial theorem statement, transforming them into subsequent intermediate goals, and ultimately discharging all proof obligations. In this work, we develop and experimentally evaluate approaches that predict the most likely tactics that will achieve particular desired transformations of proof states. First, we design several characterizations to efficiently capture the semantics of the proof transformations. Then we use them to create large datasets on which we train state-of-the-art random forests and language models. The trained models are evaluated experimentally, and we show that our best model is able to guess the right tactic for a given proof transformation in 74% of the cases. Finally, we use the trained methods in two applications: proof shortening and tactic suggesting. To the best of our knowledge, this is the first time that tactic synthesis is trained on proof transformations and assists interactive theorem proving in these ways.

---

Farah Al Wardani, [Kaustuv Chaudhuri](https://chaudhuri.info/) and Dale Miller

**Formal Reasoning using Distributed Assertions**

**Abstract:** When a proof system checks a formal proof, we can say that the kernel asserts that the formula is a theorem in a particular logic. We describe a general framework in which such assertions can be made global so that any other proof assistant willing to trust the creator of the assertion can use that assertion without rechecking any associated formal proof. This framework is heterogeneous and allows each participant to decide which tools and operators they are willing to trust in order to accept external assertions. This framework can also be integrated into existing proof systems by making minor changes to the input and output subsystems of the prover. It achieves a high level of distributivity using off-the-shelf technologies: IPFS, IPLD, and public key cryptography. We illustrate the framework by providing implementations of an intermediate tool for validating and publishing assertion objects and a modified version of the Abella theorem prover that can use and publish such assertions.

---

Ryota Haga, Yuki Kagaya and [Takahito Aoto](http://www.nue.ie.niigata-u.ac.jp/~aoto/)

**A Critical Pair Criterion for Level-Commutation of Conditional Term Rewriting Systems**

**Abstract:** The rewrite relation of a conditional term rewriting system (CTRS) can be divided into a hierarchy of rewrite relations of term rewriting systems (TRSs) by the depth of the recursive use of rewrite relation in conditions; a CTRS is said to be level-confluent if each of these TRSs are confluent, and level-confluence implies confluence. We introduce level-commutation of CTRSs that extends the notion of level-confluence, in a way similar to extending confluence to commutation, and give a critical pair criterion for level-commutation of oriented CTRSs with extra variables (3-CTRSs). Our result generalizes a criterion for commutation of TRSs of (Toyama, 1987), and properly extends a criterion for level-confluence of orthogonal oriented 3-CTRSs (Suzuki et al., 1995). We also present critical pair criteria for commutation and confluence of join and semi-equational 3-CTRSs that may have overlaps.

---

Martin Bromberger, Lorenz Leutgeb and [Christoph Weidenbach](https://www.mpi-inf.mpg.de/departments/automation-of-logic/people/christoph-weidenbach)

**Symbolic Model Construction for Saturated Constrained Horn Clauses**

**Abstract:** Clause sets saturated by hierarchic superposition do not offer an explicit model representation, rather the guarantee that all non-redundant inferences have been performed without deriving a contradiction. We present an approach to explicit model construction for saturated constrained Horn clauses. Constraints are in linear arithmetic, the first-order part is restricted to a function-free language. The model construction is effective and clauses can be evaluated with respect to the model. Furthermore, we prove that our model construction produces the least model.

---

[Sibylle Möhle](https://www.mpi-inf.mpg.de/departments/automation-of-logic/people/sibylle-moehle)

**An Abstract CNF-to-d-DNNF Compiler Based on Chronological CDCL**

**Abstract:** We present Abstract CNF2dDNNF, a calculus describing an approach for compiling a formula in conjunctive normal form (CNF) into deterministic negation normal form (d-DNNF). It combines component-based reasoning with a model enumeration approach based on conflict-driven clause learning (CDCL) with chronological backtracking. Its properties, such as soundness and termination, carry over to implementations which can be modeled by means of it. We provide a rigorous correctness proof and a detailed example. The main conceptual differences to currently available tools targeting d-DNNFs are discussed and future research directions presented. The aim of this work is to introduce a novel method for d-DNNF compilation with focus on model computation. To the best of our knowledge, our approach is the first knowledge compilation method using CDCL with chronological backtracking.

---

Chad Brown, [Adam Pease](https://www.adampease.org/) and Josef Urban

**Translating SUMO-K to Higher-Order Set Theory**

**Abstract:** We describe a translation from a fragment of SUMO (SUMO-
K) into higher-order set theory. The translation provides a formal seman-
tics for portions of SUMO which are beyond first-order and which have
previously only had an informal interpretation. It also for the first time
embeds a large common-sense ontology into a very secure interactive
theorem proving system. We further extend our previous work in finding
contradictions in SUMO from first order constructs to include a portion
of SUMO’s higher order constructs. Finally, using the translation, we can
create problems that can be proven using higher-order interactive and
automated theorem provers. This is tested in several systems and can be
used to form a corpus of higher-order common-sense reasoning problems.