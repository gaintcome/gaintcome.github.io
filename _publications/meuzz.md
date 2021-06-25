---
title: "MEUZZ: Smart Seed Scheduling for Hybrid Fuzzing"
collection: publications
permalink: /publication/meuzz
date: 2020-14-10
venue: 'Proceedings of the 23rd International Symposium on Research in Attacks, Intrusions and Defenses'
---
Yaohui Chen, Mansour Ahmadi, **Reza Mirzazade Farkhani**, Boyu Wang, Long Lu

[PDF](http://gaintcome.github.io/files/meuzz.pdf)


### Abstract

Seed scheduling is a prominent factor in determining the yields of hybrid fuzzing. Existing hybrid fuzzers schedule seeds based on fixed heuristics that aim to predict input utilities. However, such heuristics are not generalizable as there exists no one-size-fits-all rule applicable to different programs. They may work well on the programs from which they were derived, but not others. To overcome this problem, we design a Machine learning-Enhanced hybrid fUZZing system (MEUZZ), which employs supervised machine learning for adaptive and generalizable seed scheduling. MEUZZ determines which new seeds are expected to produce better fuzzing yields based on the knowledge learned from past seed scheduling decisions made on the same or similar programs. MEUZZ’s learning is based on a series of features extracted via code reachability and dynamic analysis, which incurs negligible runtime overhead (in microseconds). Moreover, MEUZZ automatically infers the data labels by evaluating the fuzzing performance of each selected seed. As a result, MEUZZ is generally applicable to, and performs well on, various kinds of programs. Our evaluation shows MEUZZ significantly outperforms the state-of-the-art grey-box and hybrid fuzzers, achieving 27.1% more code coverage than QSYM. The learned models are reusable and transferable, which boosts fuzzing performance by 7.1% on average and improves 68% of the 56 cross-program fuzzing campaigns. MEUZZ discovered 47 deeply hidden and previously unknown bugs, among which 21 were confirmed and fixed by the developers, when fuzzing 8 well-tested programs with the same configurations as used in previous work.
