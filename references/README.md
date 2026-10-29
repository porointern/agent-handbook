# Engineering reference catalog

This bibliography uses the 18 knowledge areas (KAs) of **SWEBOK v4** as its
spine, followed by fields useful for game-playing and other autonomous agents.
It is a reading aid, not a curriculum requirement, certification claim or new
delivery gate. Each project keeps its own chapter → requirement/specification/
kernel maps, reading records, decisions and empirical checks.

The starting curriculum is poroburu's York Software Engineering BEng course
list. The [York program](https://lassonde.yorku.ca/eecs/academics/undergraduate/future-students/software-engineering-beng/)
and its [2023–2024 General Stream checklist](https://lassonde.yorku.ca/wp-content/uploads/2023-2024-Degree-Checklist-BEng-Software-General.pdf)
provide course context, not proof that York assigned these books. Course numbers
are navigation labels from that starting point, not a current graduation audit.
Book selection favors useful lawful access over matching a course's textbook.
The [IEEE KA outline](https://www.computer.org/education/bodies-of-knowledge/software-engineering/topics)
owns the SWEBOK structure. S01 identifies the privately supplied revision used
for chapter navigation; appendices are not additional KAs.

## How to use the catalog

Start with the KA or specialist field, then look up its source IDs in the title
register. Each title is counted once, even when used in several KAs. The register
owns authors, edition/version, access, official URL and licence. The tables give
chosen sources, substitutes and when to reach for them. Substitutes cover the
named topic, not necessarily the whole book. Chapter titles/numbers are general
navigation only; a project claim needs its own exact version and pages actually
read. No claim of full-text review follows from this catalog.

Access classes describe the cataloged route, independently of reuse rights:

- **open**: full text offered free by an author, publisher or authorized project;
  this includes restricted personal-use texts and is not an open-licence claim.
- **paid**: obtain a lawful purchase or library loan, or use the listed substitute.
  A sample, contents page or abstract is not full-text access.
- **owner-provided**: ask the owner for an authorized private copy. Its URL cell
  says only `owner-provided`; availability is not promised on another host. This
  classification preserves the supplied route even if another legal route exists.

Licence descriptions preserve acquisition-record limits: **expected** and
**unverified** are not verified grants. Check the exact acquired version before
reuse; unknown terms authorize no redistribution. This repository contains only
bibliography and our navigation prose: no book files, extracted passages or
quotations. Code and third-party contributions may have separate terms.

## SWEBOK v4 knowledge areas

S01 is the common overview and fallback for every KA. Its chapter number equals
the KA number below. Where the starting curriculum has no dedicated course, the
nearest course context is explicit rather than inventing a course match.

| KA | York course context | Chosen sources; substitutes | When to reach for it; general chapter pointers |
| --- | --- | --- | --- |
| 1. Software Requirements | EECS 4312, Software Engineering Requirements | S02; substitute S01 ch. 1 | Elicit goals, resolve obstacles and make criteria measurable. S02 goal modeling and requirements elaboration chapters; S01 ch. 1. |
| 2. Software Architecture | EECS 3311 Software Design; EECS 4314 Advanced Software Engineering | S40 and S01 ch. 2; substitute S13 for local pattern choices | Compare component boundaries and architectural trade-offs. S40 Berkeley DB and LLVM chapters; S13 Component and Event Queue chapters. |
| 3. Software Design | EECS 3311 | S12; substitutes S13 and S01 ch. 3 | Model domain boundaries and invalid states before implementation. S12 Domain Modeling with Types and Modeling Workflows as Pipelines; S13 State and Component. |
| 4. Software Construction | EECS 2011 Fundamentals of Data Structures; EECS 3311 | S09 and S15; substitutes S13 and S01 ch. 4 | Choose maintainable implementation and data structures. S09 Code Review, Documentation and Build Systems; S15 lists, hashing and graph chapters. |
| 5. Software Testing | EECS 4313 Software Engineering Testing | S07; substitute S08 for systematic criteria, or S01 ch. 5 for the overview | Design fault-revealing inputs and interpret coverage. S07 Code Coverage, Mutation Analysis and Reducing Failure-Inducing Inputs; S08 graph, logic and input-space coverage chapters. |
| 6. Software Engineering Operations | EECS 4314; EECS 3221 Operating System Fundamentals as background | S10 and S11; substitute S01 ch. 6 | Reason about reliability objectives, incidents and recovery. S10 Service Level Objectives and Effective Troubleshooting; S11 Implementing SLOs and Incident Response. |
| 7. Software Maintenance | EECS 4314; EECS 3311 | S09; substitute S01 ch. 7 | Change long-lived software and retire obsolete interfaces. S09 Deprecation and Large-Scale Changes; S01 ch. 7. |
| 8. Software Configuration Management | EECS 4314; ENG 4000 Engineering Project context | S09; substitutes S11 for release practice and S01 ch. 8 | Identify baselines and safely deliver changes. S09 Version Control and Branch Management and Continuous Delivery; S11 Canarying Releases. |
| 9. Software Engineering Management | ENG 4000; EECS 4314, nearest project contexts | S01 ch. 9; substitute S09 for team practice | Plan, evaluate and close work with explicit uncertainty. S01 ch. 9; S09 How to Lead a Team and Measuring Engineering Productivity. |
| 10. Software Engineering Process | EECS 4314; ENG 4000 | S01 ch. 10; substitute S09 for practice examples | Choose and evaluate a lifecycle or process change. S01 ch. 10; S09 Software Engineering, Over Time and Continuous Integration. |
| 11. Software Engineering Models and Methods | EECS 3342 System Specification and Refinement | S03; substitutes S04 for Event-B refinement, S06 for model checking and S19 for state-machine modeling | Separate a model's assumptions from its guarantees. S03 chs. 2–4, 8–10 and 14; S04 refinement case studies; S06 transition systems, temporal logic and abstraction chapters; S19 state machines and refinement chapters. |
| 12. Software Quality | EECS 4313; EECS 4315 Mission-Critical Systems | S01 ch. 12 and S10; substitutes S07 for test adequacy and S05 for safety analysis | Connect quality attributes to measures and prevention. S01 ch. 12; S10 Testing for Reliability; S07 Mutation Analysis; S05 systems-theoretic hazard analysis chapters. |
| 13. Software Security | EECS 3482/4482 security context; EECS 4315 | S36; substitutes S01 ch. 13 and S10 for limited operational context | Describe opponents, trust boundaries and control assurance. S36 chs. 2, 4, 6, 10, 27–28; S10 Managing Critical State. |
| 14. Software Engineering Professional Practice | ENG 3000 Professional Engineering Practice; ENG 4000 | S01 ch. 14; substitute S09 for communication and teamwork | Clarify obligations, rights, uncertainty and accountable communication. S01 ch. 14; S09 Knowledge Sharing and Documentation. |
| 15. Software Engineering Economics | ENG 3000/4000, nearest engineering-project context; no dedicated economics course asserted | S01 ch. 15; substitutes S36 ch. 8 for security incentives and S09 for engineering trade-offs | Compare decision value, cost, risk and uncertainty. S01 ch. 15; S36 Economics; S09 Measuring Engineering Productivity. The substitutes do not cover all engineering economics. |
| 16. Computing Foundations | EECS 2011, 3101 Design and Analysis of Algorithms, 3221, 3214 Computer Networks; EECS 3421/4411 database context; EECS 4404 machine learning context | S14, S15, S32, S33 and S24; substitutes S34/S35 for data systems and S37/S38/S39 for learning foundations | Check algorithm, platform and model assumptions. S14 dynamic programming and graph chapters; S32 concurrency/persistence parts; S33 internetworking/reliability chapters; S24 search/uncertainty chapters; S34 data-model readings; S35 chs. 5–9; S37 chs. 8–12; S38 probabilistic-model chapters; S39 generalization chapters. |
| 17. Mathematical Foundations | MATH 1028 discrete mathematics, MATH 1090 logic, MATH 1025 linear algebra; CIVL 2390 probability/statistics | S29, S30, S31 and S17; substitutes S16 for probability and S37 for applied mathematical background | Check proofs, sampling and numerical representations. S29 induction, graphs and probability chapters; S30 propositional/predicate logic chapters; S31 vector spaces and linear maps; S17 inference chapters; S16 conditional probability and limit theorems; S37 chs. 2–7. |
| 18. Engineering Foundations | EECS 2032/3216 embedded/digital systems; ENG 4550 Introduction to Control Systems; EECS 4315 | S19 and S18; substitutes S05 for safety and S01 ch. 18 for breadth | Join computing to timing, feedback and engineering measurement. S19 state machines, composition, scheduling and verification chapters; S18 feedback, stability and PID chapters; S05 systems and hazard analysis chapters. |

## Fields for autonomous agents and game-playing systems

These are separate entries, not extra SWEBOK KAs. A beyond-curriculum row names
its nearest prerequisite course without claiming a dedicated York course.

| Field | York course context | Chosen sources; substitutes | When to reach for it; general chapter pointers |
| --- | --- | --- | --- |
| Planning | Beyond curriculum; EECS 3101/3342 background | S20; substitutes S24 and S25 | Relate search to actual acting and retained refinement. S20 chs. 2–5: deterministic models, refinement methods, temporal models and nondeterministic models; S25 ch. 11; S24 planning chapters. |
| Decisions under uncertainty | Beyond curriculum; CIVL 2390 background | S21; substitutes S24 and S25 | Model belief, observations and information value. S21 chs. 3, 6, 20–22; S25 chs. 12–18; S24 uncertainty and decision chapters. |
| Reinforcement learning | Beyond curriculum; EECS 4404 background | S22; substitutes S24 and S25 | Distinguish prediction, control and learning from interaction. S22 chs. 2–6, 8 and 11; S25 ch. 22; S24 reinforcement-learning chapter. |
| Multi-agent systems and game theory | Beyond curriculum; EECS 3101/4404 background | S23; substitutes S21 and S25 for decision/game introductions | Analyze strategic interaction and opponent adaptation. S23 normal-form games, extensive-form games and multiagent-learning chapters; S21 multiagent chapters; S25 chs. 5 and 18. |
| Optimization | Beyond curriculum; MATH 1025 and EECS 3101 background | S26 and S27; substitute S37 ch. 7 for background | Establish feasibility and mathematical assumptions before choosing a solver. S26 chs. 2–5 and 9–11; S27 constraints, discrete optimization and uncertainty chapters. |
| Embedded and cyber-physical systems | EECS 2032/3216; ENG 4550 | S19, a first-priority reference; substitutes S18 for control and S03 for temporal specification | Reason about concurrent state, deadlines and environmental feedback. S19 state machines, composition, scheduling, temporal logic, refinement and reachability chapters; S18 feedback/stability chapters; S03 chs. 8–10. |
| AI foundations | Beyond curriculum; EECS 3101/4404 background | S24; substitute S25 | Share vocabulary across search, inference, planning and learning. S24 corresponding topic chapters; S25 chs. 3–6, 11–22. |
| Game AI practice | Beyond curriculum; EECS 3311/3101 background | S28; substitutes S13 for patterns and S24 for AI theory | Connect movement and decision structures to a game's constraints. S28 Movement, Decision Making, Tactical and Strategic AI; S13 Game Loop, Update Method and State; S24 search/planning chapters. |

## Title register

Metadata combines official landing pages checked on 2026-10-29 with supplied
acquisition and reading records; unresolved terms stay explicit. A version below
is deliberately selected, not a claim to be the
latest edition. Living websites require a dated snapshot and hash at acquisition.
The private-library format is [specified separately](private-library.md).

| ID | Title; authors/editors | Edition/version; year | Access | Official URL | Licence / acquisition limit |
| --- | --- | --- | --- | --- | --- |
| S01 | Guide to the Software Engineering Body of Knowledge; Hironori Washizaki (ed.), IEEE Computer Society | v4.0a; v4 first published 2024; supplied revision date unverified | owner-provided | owner-provided | IEEE copyright; private supplied copy. Free account-based access does not imply a reuse licence. |
| S02 | Requirements Engineering: From System Goals to UML Models to Software Specifications; Axel van Lamsweerde | 1st ed.; 2009 | paid | [Wiley](https://www.wiley.com/en-us/Requirements+Engineering%3A+From+System+Goals+to+UML+Models+to+Software+Specifications-p-9780470012703) | Publisher copyright; purchase/loan terms, no open reuse grant established. |
| S03 | Specifying Systems; Leslie Lamport | 1st ed.; 2002; author PDF revision 2008 | open | [Author](https://lamport.azurewebsites.net/tla/book.html) | Pearson copyright; author page permits personal use, other reproduction/distribution needs permission. |
| S04 | Modeling in Event-B: System and Software Engineering; Jean-Raymond Abrial | 1st ed.; 2010 | paid | [Cambridge](https://www.cambridge.org/core/books/modeling-in-event-b/F39FF5F1B60F0AA585718B8E6A4F9DD7) | Publisher copyright; purchase/loan terms, no open reuse grant established. |
| S05 | Engineering a Safer World; Nancy G. Leveson | 1st ed.; 2012 | owner-provided | owner-provided | CC BY-NC-ND 4.0 identified in supplied publisher-licence record; exact supplied-byte/version match unverified. |
| S06 | Principles of Model Checking; Christel Baier and Joost-Pieter Katoen | 1st ed.; 2008 | paid | [MIT Press](https://mitpress.mit.edu/9780262026499/principles-of-model-checking/) | Publisher copyright; purchase/loan terms, no open reuse grant established. |
| S07 | The Fuzzing Book; Andreas Zeller, Rahul Gopinath, Marcel Böhme, Gordon Fraser and Christian Holler | Living web edition; snapshot date required | open | [Author project](https://www.fuzzingbook.org/) | Text CC BY-NC-SA 4.0; associated code MIT. |
| S08 | Introduction to Software Testing; Paul Ammann and Jeff Offutt | 2nd ed.; 2016 | paid | [Cambridge](https://www.cambridge.org/highereducation/books/introduction-to-software-testing/95E57CCADEA697EC8594F03729F47311) | Publisher copyright; purchase/loan terms, no open reuse grant established. |
| S09 | Software Engineering at Google; Titus Winters, Tom Manshreck and Hyrum Wright (eds.) | 1st ed.; 2020 | open | [Abseil](https://abseil.io/resources/swe-book) | Online text CC BY-NC-ND 4.0. |
| S10 | Site Reliability Engineering; Betsy Beyer, Chris Jones, Jennifer Petoff and Niall Richard Murphy (eds.) | 1st ed.; 2016; not the newer second edition | open | [Google](https://sre.google/sre-book/table-of-contents/) | Online reuse licence unverified here; record the acquired copy's terms. Free reading alone grants no redistribution rights. |
| S11 | The Site Reliability Workbook; Betsy Beyer, Niall Richard Murphy, David K. Rensin, Kent Kawahara and Stephen Thorne (eds.) | 1st ed.; 2018 | open | [Google](https://sre.google/workbook/table-of-contents/) | Online reuse licence unverified here; record the acquired copy's terms. Free reading alone grants no redistribution rights. |
| S12 | Domain Modeling Made Functional; Scott Wlaschin | 1st ed.; 2018 | paid | [Pragmatic Bookshelf](https://pragprog.com/titles/swdddf/domain-modeling-made-functional/) | Publisher copyright; purchase/loan terms, no open reuse grant established. |
| S13 | Game Programming Patterns; Robert Nystrom | 1st ed.; 2014 | open | [Author](https://gameprogrammingpatterns.com/) | Free online reading; reuse licence unverified here. Preserve copyright and check exact terms before reuse. |
| S14 | Algorithms; Jeff Erickson | 1st ed.; June 2019 | open | [Author](https://jeffe.cs.illinois.edu/teaching/algorithms/) | Book CC BY 4.0; other lecture notes have different terms. |
| S15 | Open Data Structures; Pat Morin | Java edition; 2013 print edition, dated web/PDF revision required | open | [Author](https://opendatastructures.org/) | CC BY 2.5 expected in acquisition record; verify version-specific deed at acquisition. |
| S16 | Introduction to Probability; Joseph K. Blitzstein and Jessica Hwang | 1st ed.; 2014; do not silently substitute second-edition locators | owner-provided | owner-provided | Private copy only; supplied record identifies first edition, no redistribution grant established. |
| S17 | OpenIntro Statistics; David M. Diez, Mine Çetinkaya-Rundel and Christopher D. Barr | 4th ed.; 2019 | open | [OpenIntro](https://www.openintro.org/book/os/) | CC BY-SA 3.0 expected; verify the selected file's notice. |
| S18 | Feedback Systems; Karl J. Åström and Richard M. Murray | 2nd ed.; 2021 publication; supplied public manuscript 24 July 2020, release 3.1.5 | owner-provided | owner-provided | Personal use only in supplied licence record; reproduction needs publisher consent; no byte comparison established. |
| S19 | Introduction to Embedded Systems: A Cyber-Physical Systems Approach; Edward A. Lee and Sanjit A. Seshia | 2nd ed.; 2017; digital v2.3 | open | [Authors](https://ptolemy.berkeley.edu/books/leeseshia/) | All rights reserved; authorized author PDF, private reading copy. |
| S20 | Automated Planning and Acting; Malik Ghallab, Dana Nau and Paolo Traverso | 1st ed.; 2016; supplied chapter set | owner-provided | owner-provided | Cambridge copyright; authorized private study; no redistribution. An earlier belief in open author-PDF access is not treated as established. |
| S21 | Algorithms for Decision Making; Mykel J. Kochenderfer, Tim A. Wheeler and Kyle H. Wray | 1st ed.; 2022; supplied PDF build 20 September 2026 | owner-provided | owner-provided | CC BY-NC-ND identified by private reading record; deed version unverified in acquisition ledger. |
| S22 | Reinforcement Learning: An Introduction; Richard S. Sutton and Andrew G. Barto | 2nd ed.; 2018; supplied PDF revision not byte-matched to official source | owner-provided | owner-provided | CC BY-NC-ND 4.0 identified in supplied publisher-licence record; exact PDF revision unverified. |
| S23 | Multiagent Systems: Algorithmic, Game-Theoretic, and Logical Foundations; Yoav Shoham and Kevin Leyton-Brown | 1st ed.; 2009 | open | [Authors](https://www.masfoundations.org/) | Free author download; licence unknown in acquisition ledger, no redistribution grant established. |
| S24 | Artificial Intelligence: Foundations of Computational Agents; David L. Poole and Alan K. Mackworth | 3rd ed.; 2023 | open | [Authors](https://artint.info/) | Authorized full-text HTML; reuse terms unverified here. |
| S25 | Artificial Intelligence: A Modern Approach; Stuart Russell and Peter Norvig | 4th US ed.; 2021 | paid | [Authors](https://aima.cs.berkeley.edu/) | Pearson copyright; purchase/loan terms. Free companion materials do not supply the full book. |
| S26 | Convex Optimization; Stephen Boyd and Lieven Vandenberghe | 1st ed.; 2004; private reading record used seventh printing with corrections, 2009 | open | [Authors](https://web.stanford.edu/~boyd/cvxbook/) | Cambridge copyright; author hosting permitted by publisher; no open redistribution grant established. |
| S27 | Algorithms for Optimization; Mykel J. Kochenderfer and Tim A. Wheeler | 1st ed.; 2019; select first-edition download, not second-edition preview | open | [Authors](https://algorithmsbook.com/optimization/) | Author page identifies CC BY-NC-ND for shared PDFs; record exact deed/version at acquisition. |
| S28 | AI for Games; Ian Millington | 3rd ed.; 2019 | paid | [Routledge](https://www.routledge.com/Artificial-Intelligence-for-Games/Millington/p/book/9780367670566) | Publisher copyright; purchase/loan terms, no open reuse grant established. |
| S29 | Mathematics for Computer Science; Eric Lehman, F. Thomson Leighton and Albert R. Meyer | MIT 6.042 Spring 2018 revision | open | [MIT course source](https://courses.csail.mit.edu/6.042/spring18/mcs.pdf) | CC BY-SA 3.0 US expected in acquisition record; verify exact revision's notice. |
| S30 | forall x: Calgary; P. D. Magnus, Tim Button, J. Robert Loftis, Aaron Thomas-Bolduc and Richard Zach | Calgary rolling edition; select dated release at acquisition | open | [Open Logic Project](https://forallx.openlogicproject.org/) | CC BY 4.0; verify exceptions and exact release credits. |
| S31 | Linear Algebra Done Right; Sheldon Axler | 4th ed.; 2024 | open | [Author](https://linear.axler.net/) | CC BY-NC 4.0 expected in acquisition record; verify selected file. |
| S32 | Operating Systems: Three Easy Pieces; Remzi H. Arpaci-Dusseau and Andrea C. Arpaci-Dusseau | v1.10; 2023 | open | [Authors](https://pages.cs.wisc.edu/~remzi/OSTEP/) | Author copyright; free individual chapter PDFs, paid convenience compilation. No broad reuse grant established here. |
| S33 | Computer Networks: A Systems Approach; Larry L. Peterson and Bruce S. Davie | 6th ed.; 2021; dated online revision required | open | [Author project](https://book.systemsapproach.org/) | CC BY 4.0 expected for online text; verify selected release and third-party exceptions. |
| S34 | Readings in Database Systems; Peter Bailis, Joseph M. Hellerstein and Michael Stonebraker (eds.) | 5th ed.; 2015 | owner-provided | owner-provided | Editorial material CC BY-NC-SA 4.0 in supplied record; individual readings retain their own rights. The companion reading list is not a full-text paper corpus. |
| S35 | Designing Data-Intensive Applications; Martin Kleppmann | 1st ed.; 2017 | paid | [Author](https://dataintensive.net/) | O'Reilly copyright; purchase/loan terms, no open reuse grant established. |
| S36 | Security Engineering; Ross Anderson | 3rd ed.; 2020 | open | [Author archive](https://www.cl.cam.ac.uk/archive/rja14/book.html) | Authorized free chapter/full-book downloads; publisher copyright, no open reuse grant established here. |
| S37 | Mathematics for Machine Learning; Marc Peter Deisenroth, A. Aldo Faisal and Cheng Soon Ong | 1st ed.; 2020; dated PDF revision required | open | [Authors](https://mml-book.github.io/) | Cambridge copyright; author PDF available, licence unknown in acquisition ledger. |
| S38 | Pattern Recognition and Machine Learning; Christopher M. Bishop | 1st ed.; 2006 | owner-provided | owner-provided | Springer copyright, all rights reserved in supplied record; official free availability is not a CC reuse licence; exact supplied-byte match unverified. |
| S39 | Dive into Deep Learning; Aston Zhang, Zachary C. Lipton, Mu Li and Alexander J. Smola | 2023 published edition; dated online revision required | open | [Authors](https://d2l.ai/) | Text CC BY-SA 4.0, code Apache 2.0 expected; verify selected version and exceptions. |
| S40 | The Architecture of Open Source Applications; Amy Brown and Greg Wilson (eds.) | Volume 1; 2011 | open | [Editors' project](https://aosabook.org/en/) | Text CC BY 3.0; verify chapter exceptions and separate code terms. |

## Maintaining this bibliography

Keep bibliographic metadata and general navigation here. Keep project decisions,
requirement/specification/kernel mappings, claims checked and page ranges read in
the owning project. Preserve edition differences and unresolved licence facts.
Confirm access and the redirect chain when acquiring a copy; a working landing
page is not an acquisition receipt. Prefer an open substitute while a paid or
owner-provided work is unavailable. Do not fetch or publish book content as part
of maintaining this catalog.
