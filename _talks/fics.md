---
title: "Finding Bugs Using Your Own Code: Machine Learning-based Inconsistent Code Detection."
collection: talks
type: "Conference proceedings talk"
permalink: /talks/fics
venue: "OWASP Boston Application Security Conference (BASC) 2019"
date: 2019-10-19
location: "Burlington, MA"
---

By: [Mansour Ahmadi](https://www.linkedin.com/in/mansourahmadi/), Reza Mirzazade Farkhani

Machine learning has shown success in detecting known types of software vulnerabilities in recent years, but they mostly need extensive specimens to train their models.As a new alternative to such approaches, we present a learning-based technique that can identify potentially buggy code snippets which deviate from most of the code snippets implementing similar functionalities. Our approach learns from a codebase itself without the need for the cumbersome task of gathering and cleansing training samples. The core idea is that various kinds of bugs can be viewed as inconsistencies that deviate from non-buggy code that implement the same or similar logic.More specifically, we design a two-step clustering technique to find functionally-similar yet inconsistent code in software. We implemented our system on top of LLVM, which makes our approach language-agnostic.We evaluated our tool on 4 popular open source security software codebases, such as OpenSSL, OpenSSH, WolfSSL, and Mbedtls. Our tool discovered 10 new unique deep bugs, despite that some of these codebases are constantly undergoing vulnerability scans. All of the bugs have been confirmed by their developers and later fixed by either our pull requests or the developers.How does the system work really? How easy to find bugs by our approach and how much manual effort does it need? What is a proper code granularity for detecting inconsistencies?
